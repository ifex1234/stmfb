<script setup lang="ts">
import {
  about1,
  about2,
  about3,
  about4,
  about5,
  about6,
} from "~/assets/lib/about";
import { HOD1, HOD2, HOD3, HOD4 } from "~/assets/lib/HOD";
import { Board1, Board2, Board3, Board4, Board5 } from "~/assets/lib/board";
import {
  advisor1,
  advisor2,
  advisor3,
  advisor4,
  advisor5,
  advisor6,
} from "~/assets/lib/advisor";
import {
  partner1,
  partner2,
  partner3,
  partner4,
  partner5,
  partner6,
} from "~/assets/lib/partner";
</script>
<template>
  <div class="bg-white">
    <div class="pt-20 px-12 w-full">
      <h1 class="text-3xl font-bold mb-4">
        About Shepherd Trust Microfinance Bank
      </h1>
      <p class="mb-4 text-gray-500 md:w-1/2">
        Established in 2011, Shepherd Trust Microfinance Bank has grown to
        become a leading provider of financial services to Nigeria's micro,
        small, and medium enterprises. Our success is built on a foundation of
        strong corporate governance, regulatory compliance, and a deep
        commitment to responsible banking practices.
      </p>
    </div>
    <div class="px-12 pb-20 grid gap-8 md:grid-cols-3 grid-cols-1 mt-12">
      <AboutCard
        :imageSrc="about1.imageSrc"
        :title="about1.title"
        :description="about1.content"
      />
      <AboutCard
        :imageSrc="about2.imageSrc"
        :title="about2.title"
        :description="about2.content"
      />
      <AboutCard
        :imageSrc="about3.imageSrc"
        :title="about3.title"
        :description="about3.content"
        :listItms="about3.listItems"
      />
      <AboutCard
        :imageSrc="about4.imageSrc"
        :title="about4.title"
        :description="about4.content"
        :paragraphItems="about4.paragraphItems"
      />
      <AboutCard
        :imageSrc="about5.imageSrc"
        :title="about5.title"
        :description="about5.content"
      />
      <AboutCard
        :imageSrc="about6.imageSrc"
        :title="about6.title"
        :description="about6.content"
        :listItms="about6.listItems"
      />
    </div>
    <div class="bg-gray-100 lg:w-11/12 w-full mx-auto py-10 px-6 rounded-sm">
      <div
        class="space-y-4 mb-10 place-content-center place-items-center mt-10"
      >
        <h4 class="text-3xl font-semibold text-center">Our Leadership Team</h4>
        <p class="text-gray-600 max-w-3xl">
          Meet the experienced professionals leading Shepherd Trust Microfinance
          Bank towards a future of innovative banking solutions.
        </p>
      </div>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        <HODcard
          :name="HOD1.name"
          :bio="HOD1.bio"
          :position="HOD1.title"
          :imageSrc="HOD1.imageUrl"
        />
        <HODcard
          :name="HOD2.name"
          :bio="HOD2.bio"
          :position="HOD2.title"
          :imageSrc="HOD2.imageUrl"
        />
        <HODcard
          :name="HOD3.name"
          :bio="HOD3.bio"
          :position="HOD3.title"
          :imageSrc="HOD3.imageUrl"
        />
        <HODcard
          :name="HOD4.name"
          :bio="HOD4.bio"
          :position="HOD4.title"
          :imageSrc="HOD4.imageUrl"
        />
      </div>
      <div
        class="space-y-4 mb-10 place-content-center place-items-center mt-10"
      >
        <h4 class="text-3xl font-semibold text-center">Board of Directors</h4>
        <p class="text-gray-600 max-w-3xl">
          Our distinguished board members bring decades of experience and
          expertise to guide our strategic direction.
        </p>
      </div>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <BoardCard
          :name="Board1.name"
          :bio="Board1.bio"
          :position="Board1.designation"
        />
        <BoardCard
          :name="Board2.name"
          :bio="Board2.bio"
          :position="Board2.designation"
        />
        <BoardCard
          :name="Board3.name"
          :bio="Board3.bio"
          :position="Board3.designation"
        />
        <BoardCard
          :name="Board4.name"
          :bio="Board4.bio"
          :position="Board4.designation"
        />
        <BoardCard
          :name="Board5.name"
          :bio="Board5.bio"
          :position="Board5.designation"
        />
      </div>
    </div>
    <div
      class="grid grid-cols-1 md:grid-cols-2 px-4 md:px-4 lg:px-12 pt-5 bg-gray-100 lg:w-11/12 w-full mx-auto"
    >
      <div class="flex flex-col p-5 gap-y-3">
        <span class="space-y-3"
          ><h5 class="font-semibold text-xl text-center">
            Advisors and Partners
          </h5>
          <p class="text-center text-gray-500">
            Working together with trusted institutions to serve you better.
          </p></span
        >
        <span
          class="md:p-6 p-2 space-y-4 outline-offset-2 outline-gray-400 border border-gray-300 focus:outline-2 rounded-md"
          ><AdvisorCard
            :name="advisor1.name"
            :role="advisor1.role"
            :imageUrl="advisor1.url"
          />

          <AdvisorCard
            :name="advisor2.name"
            :role="advisor2.role"
            :imageUrl="advisor2.url"
          />
          <AdvisorCard
            :name="advisor3.name"
            :role="advisor3.role"
            :imageUrl="advisor3.url"
          />
          <AdvisorCard
            :name="advisor4.name"
            :role="advisor4.role"
            :imageUrl="advisor4.url"
          />
          <AdvisorCard
            :name="advisor5.name"
            :role="advisor5.role"
            :imageUrl="advisor5.url"
          />
          <AdvisorCard
            :name="advisor6.name"
            :role="advisor6.role"
            :imageUrl="advisor6.url"
          />
        </span>
      </div>
      <div class="flex flex-col p-5 gap-y-3">
        <span class="space-y-3">
          <h5 class="font-semibold text-xl text-center">Our Bankers</h5>
          <p class="text-center text-gray-500">
            Supported by Nigeria's leading financial institutions.
          </p></span
        >

        <span
          class="p-6 grid grid-cols-2 space-y-4 space-x-3 outline-offset-2 outline-gray-400 border border-gray-300 focus:outline-2 rounded-md"
        >
          <PartnerCard :imageUrl="partner1.url" :name="partner1.name" />
          <PartnerCard
            :imageUrl="partner2.url"
            :name="partner2.name"
          /><PartnerCard
            :imageUrl="partner3.url"
            :name="partner3.name"
          /><PartnerCard
            :imageUrl="partner4.url"
            :name="partner4.name"
          /><PartnerCard
            :imageUrl="partner5.url"
            :name="partner5.name"
          /><PartnerCard :imageUrl="partner6.url" :name="partner6.name" />
        </span>
      </div>
    </div>
  </div>
</template>
