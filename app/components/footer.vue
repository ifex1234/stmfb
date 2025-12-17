<template>
  <div class="bg-gray-800 w-full md:h-86 mt-10">
    <div
      class="grid grid-cols-1 md:grid-cols-4 gap-2 w-11/12 mx-auto pt-10 mb-10"
    >
      <div class="flex flex-col gap-y-3">
        <span class="font-semibold text-xl mr-3 text-gray-200"
          >Shepherd Trust
        </span>
        <span class="text-gray-400 text-sm"
          >Your trusted partner in microfinance banking services.</span
        >
        <img
          src="../assets/images/ndpr-DGf25P_L.png"
          class="h-18 w-18"
          alt=""
        />
      </div>
      <div class="flex flex-col gap-y-2">
        <p class="text-gray-100">Quick Links</p>
        <NuxtLink
          class="text-gray-200 text-sm mt-2.5 hover:underline"
          to="/about"
          >About Us</NuxtLink
        >
        <NuxtLink class="text-gray-200 text-sm hover:underline" to="/services"
          >Services</NuxtLink
        >
        <NuxtLink class="text-gray-200 text-sm hover:underline" to="/contact"
          >Contact</NuxtLink
        >
      </div>
      <div>
        <p class="text-gray-100">Contact Us</p>
        <p class="text-gray-200 text-sm mt-2.5 pt-2">
          12, Oladele Kadiri Close <br />
          Off Nob-Oluwa St., Ogba <br />
          Lagos, Nigeria
        </p>
        <p class="text-gray-200 text-sm py-3">Phone: +234 (0)808-125-0499</p>
        <p class="text-gray-200 text-sm">Email: info@stmfb.com</p>
      </div>

      <div class="flex flex-col ml-0 md:ml-20 mt-6 md:mt-0 text-gray-50">
        <p class="mb-2">Newsletter</p>
        <input
          type="text"
          placeholder="Enter your email"
          class="p-2 rounded-md mb-2 w-full"
        />
        <button class="bg-white text-black p-2 rounded-md w-full">
          Subscribe
        </button>
      </div>
    </div>
    <div
      class="border-t border-gray-500 w-11/12 mx-auto my-6 h-20 flex items-center justify-center"
    >
      <p class="text-center text-gray-200 text-sm">
        © 2025 Shepherd Trust Microfinance Bank. All rights reserved.
      </p>
    </div>
  </div>
</template>
