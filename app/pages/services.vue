<script setup lang="ts">
import {
  product1,
  product2,
  product3,
  product4,
  product5,
} from "~/assets/lib/loanProduct";
import {
  neoProducts,
  neoProducts2,
  neoProducts3,
} from "~/assets/lib/neocollect";
import Card2 from "~/components/card2.vue";
</script>
<template>
  <div class="px-4 py-5 bg-white">
    <div class="space-y-4 mb-10 place-content-center place-items-center mt-10">
      <h4 class="text-3xl font-semibold text-center">Our Services</h4>
      <p class="text-gray-600 max-w-3xl">
        Comprehensive financial solutions designed to support your business
        <br class="hidden md:block" />
        growth and personal financial goals.
      </p>
    </div>
    <div class="px-5 md:px-4 lg:px-10">
      <span class="w-full space-y-4">
        <span class="flex flex-row space-x-3 items-center">
          <img src="../assets//images/mobile.png" alt="" />
          <h4 class="text-xl md:text-3xl font-semibold">
            NeoCash Mobile App
          </h4></span
        >

        <p class="w-full lg:w-2/4 text-gray-500">
          Your Bank in Your Pocket - NeoCash brings the full power of Shepherd
          Trust Microfinance Bank to your mobile device, enabling you to manage
          your business finances anytime, anywhere. As part of our commitment to
          making banking more accessible, we've designed NeoCash to be intuitive
          and efficient.
        </p>
      </span>
    </div>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-6 md:px-2 lg:px-10 mt-10">
      <div
        class="p-6 outline-offset-2 outline-gray-400 border border-gray-300 focus:outline-2 rounded-md"
      >
        <h4 class="text-2xl font-medium mb-4">Digital Loan Applications</h4>
        <p class="text-gray-500">
          Submit loan applications directly through the app, with minimal
          documentation required. Our intelligent processing system helps
          deliver faster decisions while maintaining our commitment to
          responsible lending.
        </p>
      </div>
      <div
        class="p-6 outline-offset-2 outline-gray-400 border border-gray-300 focus:outline-2 rounded-md"
      >
        <h4 class="text-2xl font-medium mb-4">Account Management</h4>
        <p class="text-gray-500">
          Monitor your balances, track transactions, and manage your savings
          goals seamlessly. Whether you're running a market stall or managing
          multiple business locations, NeoCash gives you complete visibility of
          your finances.
        </p>
      </div>
      <div
        class="p-6 outline-offset-2 outline-gray-400 border border-gray-300 focus:outline-2 rounded-md"
      >
        <h4 class="text-2xl font-medium mb-4">Secure Payments</h4>
        <p class="text-gray-500">
          Transfer funds, pay bills, and manage vendor payments securely through
          our encrypted platform. Every transaction is protected by
          industry-leading security protocols and backed by our dedicated
          support team.
        </p>
      </div>
    </div>
    <div
      class="lg:w-11/12 mx-auto mt-10 md:px-4 lg:px-10 space-y-4 outline-offset-2 outline-gray-400 border border-gray-300 focus:outline-2 rounded-md p-6"
    >
      <h4 class="text-lg font-medium">Getting Started with NeoCash</h4>
      <p class="text-gray-500">
        Download the app from your preferred app store, complete our streamlined
        registration process, and begin banking with enhanced convenience. Our
        support team is available to guide you through the setup process if
        needed.
      </p>
      <NuxtLink
        to="/www.neochash.ng"
        class="inline-block bg-black text-white px-4 py-2 rounded-md hover:bg-gray-800"
        >Download NeoCash</NuxtLink
      >
    </div>

    <div class="px-4 md:px-2 lg:px-12 mt-20">
      <span class="w-full space-y-4">
        <span class="flex flex-row space-x-3 items-center">
          <img src="../assets//images/finance.png" alt="" />
          <h4 class="text-xl md:text-3xl font-semibold">NeoCollect</h4></span
        >

        <p class="w-full md:w-3/5 text-gray-500">
          Empowering Lenders with Advanced Collection Technology - NeoCollect
          represents our commitment to strengthening Nigeria's lending
          ecosystem. This comprehensive platform enables financial institutions
          to streamline their loan collection processes through automated direct
          debit management and advanced tracking capabilities.
        </p>
      </span>
      <div
        class="grid grid-cols-1 md:grid-cols-3 gap-6 md:px-10 mt-10 md:-ml-10"
      >
        <!-- <div
          class="p-2 md:p-6 outline-offset-2 outline-gray-400 border border-gray-300 focus:outline-2 rounded-md"
        >
          <h4 class="md:text-2xl text-xl font-medium mb-4">
            Direct Debit Management
          </h4>
          <ul class="list-disc list-inside space-y-2">
            <li>Real-time mandate status monitoring</li>
            <li>Automated mandate setup and activation</li>
            <li>Flexible collection scheduling</li>
            <li>Instant notification system</li>
          </ul>
        </div> -->

        <Card2 :title="neoProducts.title" :listItems="neoProducts.listItems" />
        <Card2
          :title="neoProducts2.title"
          :listItems="neoProducts2.listItems"
        />
        <Card2
          :title="neoProducts3.title"
          :listItems="neoProducts3.listItems"
        />

        <!-- <div
          class="p-2 md:p-6 outline-offset-2 outline-gray-400 border border-gray-300 focus:outline-2 rounded-md"
        >
          <h4 class="md:text-2xl text-xl font-medium mb-4">
            Advanced Analytics
          </h4>
          <ul class="list-disc list-inside space-y-2">
            <li>Comprehensive collection reporting</li>
            <li>Performance analytics dashboard</li>
            <li>Risk monitoring tools</li>
            <li>Collection efficiency metrics</li>
          </ul>
        </div> -->

        <!-- <div
          class="p-2 md:p-6 outline-offset-2 outline-gray-400 border border-gray-300 focus:outline-2 rounded-md"
        >
          <h4 class="md:text-2xl text-xl font-medium mb-4">API Integration</h4>
          <ul class="list-disc list-inside space-y-2">
            <li>Secure REST APIs</li>
            <li>Seamless integration with existing systems</li>
            <li>Comprehensive documentation</li>
            <li>Developer support</li>
          </ul>
        </div> -->
      </div>
    </div>
    <div
      class="md:w-11/12 mx-auto mt-10 md:px-2 lg:px-10 space-y-4 outline-offset-2 outline-gray-400 border border-gray-300 focus:outline-2 rounded-md p-6"
    >
      <h4 class="text-lg font-medium">Why Choose NeoCollect?</h4>

      <div class="grid grid-cols-1 md:grid-cols-3 mb-4 gap-y-6">
        <div>
          <h4 class="text-lg font-medium">Built on Experience</h4>
          <p class="text-gray-500">
            Drawing from our decade-plus experience in microfinance, NeoCollect
            incorporates best practices in loan collection while addressing the
            unique challenges of the Nigerian market.
          </p>
        </div>
        <div>
          <h4 class="text-lg font-medium">Regulatory Compliant</h4>
          <p class="text-gray-500">
            Fully aligned with CBN regulations and NDIC requirements, ensuring
            your collection processes meet all statutory obligations.
          </p>
        </div>
        <div>
          <div>
            <h4 class="text-lg font-medium">Scalable Solution</h4>
            <p class="text-gray-500">
              Whether you're handling hundreds or thousands of loans, NeoCollect
              scales to meet your operational needs while maintaining
              performance and reliability.
            </p>
          </div>
        </div>
      </div>
    </div>
    <div
      class="md:w-11/12 mx-auto mt-10 md:px-10 space-y-4 outline-offset-2 outline-gray-400 border border-gray-300 focus:outline-2 rounded-md p-6"
    >
      <h4 class="text-lg font-medium">Partnership Opportunities</h4>
      <p class="text-gray-500">
        We invite financial institutions to explore how NeoCollect can enhance
        their loan collection efficiency. Our team is available to discuss
        customization options and integration requirements specific to your
        organization.
      </p>
      <NuxtLink
        to="/www.neochash.ng"
        class="inline-block bg-black text-white px-4 py-2 rounded-md hover:bg-gray-800"
        >Contact Sales Team</NuxtLink
      >
    </div>
    <div class="px-4 md:px-2 lg:px-12 mt-20">
      <h4 class="text-xl font-semibold">Loan Products</h4>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-6 lg:px-4 md:px-5 mt-10">
        <Card
          :imageURL="product1.imageURL"
          :tile="product1.title"
          :description="product1.description"
          :listItems="product1.listItems"
        />
        <Card
          :imageURL="product2.imageURL"
          :tile="product2.title"
          :description="product2.description"
          :listItems="product2.listItems"
        />
        <Card
          :imageURL="product3.imageURL"
          :tile="product3.title"
          :description="product3.description"
          :listItems="product3.listItems"
        />
        <Card
          :imageURL="product4.imageURL"
          :tile="product4.title"
          :description="product4.description"
          :listItems="product4.listItems"
        />
        <Card
          :imageURL="product5.imageURL"
          :tile="product5.title"
          :description="product5.description"
          :listItems="product5.listItems"
        />
      </div>
    </div>
  </div>
</template>
