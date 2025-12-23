<script setup lang="ts">
import * as z from "zod";
import type { FormSubmitEvent } from "@nuxt/ui";

const schema = z.object({
  email: z.email("Invalid email"),
  password: z
    .string("Password is required")
    .min(8, "Must be at least 8 characters"),
});
const value = ref("");

type Schema = z.output<typeof schema>;

const state = reactive<Partial<Schema>>({
  email: undefined,
  password: undefined,
});

const toast = useToast();
async function onSubmit(event: FormSubmitEvent<Schema>) {
  toast.add({
    title: "Success",
    description: "The form has been submitted.",
    color: "success",
  });
  console.log(event.data);
}
</script>

<template>
  <UForm
    :schema="schema"
    :state="state"
    class="space-y-4 border border-gray-300 mb-5 rounded-md p-5"
    @submit="onSubmit"
  >
    <h5 class="py-3 text-2xl font-medium">Get in touch</h5>
    <label for="name">Name</label>
    <input
      type="text"
      class="w-full h-10 bg-transparent border border-gray-300 mb-5 rounded-md"
    />
    <label for="name">Email</label>
    <input
      type="text"
      class="w-full h-10 bg-transparent border border-gray-300 mb-2 rounded-md"
    />
    <label for="name">Email</label>
    <input
      type="number"
      class="w-full h-10 bg-transparent border border-gray-300 mb-2 rounded-md"
    />
    <textarea class="w-full h-32 border border-gray-300 mb-2 rounded-md" />

    <button class="w-full h-10 my-3 rounded-md text-white bg-gray-800">
      Send a message
    </button>
  </UForm>
</template>
