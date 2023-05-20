<template>
  <header class="flex items-center justify-between py-4 px-6 bg-white">
    <div class="flex items-center space-x-4">
      <img src="/path/to/logo.png" alt="Logo" class="h-8 w-auto" />
      <input
        type="text"
        placeholder="Search for collections, NFTs or users"
        class="py-2 px-3 rounded-md bg-gray-100 text-white sm:w-64 md:w-80 lg:w-96"
      />
    </div>
    <nav class="hidden md:flex space-x-4 px-2 font-semibold text-15">
      <NuxtLink to="/" class="text-gray-800">Homepage</NuxtLink>
      <NuxtLink to="/about" class="text-gray-800">About</NuxtLink>
      <NuxtLink to="/contact" class="text-gray-800">Contact</NuxtLink>
    </nav>
    <div class="hidden md:flex space-x-2 px-4">
      <button
        class="text-gray-800 bg-blue-500 hover:bg-blue-600 py-2 px-4 rounded text-15"
      >
        Sign Up
      </button>
      <button
        class="text-white bg-gray-800 hover:bg-gray-700 py-2 px-4 rounded"
      >
        Sign In
      </button>
    </div>
    <button
      class="md:hidden text-white focus:outline-none"
      @click="toggleMobileMenu"
    >
      <svg
        class="h-6 w-6"
        fill="none"
        stroke="currentColor"
        viewBox="0 0 24 24"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M4 6h16M4 12h16M4 18h16"
        ></path>
      </svg>
    </button>
    <div
      class="md:hidden absolute top-16 right-0 bg-gray-900 text-white w-48 py-2 px-4 rounded shadow-xl"
      :class="{ hidden: !isMobileMenuOpen }"
    >
      <NuxtLink
        to="/"
        class="block text-white hover:bg-gray-800 py-2"
        @click="closeMobileMenu"
      >
        Homepage
      </NuxtLink>
      <NuxtLink
        to="/about"
        class="block text-white hover:bg-gray-800 py-2"
        @click="closeMobileMenu"
      >
        About
      </NuxtLink>
      <NuxtLink
        to="/contact"
        class="block text-white hover:bg-gray-800 py-2"
        @click="closeMobileMenu"
      >
        Contact
      </NuxtLink>
      <div class="space-y-2 mt-4">
        <button
          class="text-white bg-blue-500 hover:bg-blue-600 py-2 px-4 rounded"
        >
          Sign Up
        </button>
        <button
          class="text-white bg-gray-800 hover:bg-gray-700 py-2 px-4 rounded"
        >
          Sign In
        </button>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      isMobileMenuOpen: false,
    };
  },
  methods: {
    toggleMobileMenu() {
      this.isMobileMenuOpen = !this.isMobileMenuOpen;
    },
    closeMobileMenu() {
      this.isMobileMenuOpen = false;
    },
  },
};
</script>
