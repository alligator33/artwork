<template>
  <!-- <div>
    <NuxtLink to="/"> Homepage </NuxtLink>
    <NuxtLink to="/about"> Aboutpage </NuxtLink>
    <NuxtLink to="/contact"> Contactpage </NuxtLink>
  </div> -->

  <header class="flex items-center justify-between py-4 px-6 bg-gray-900">
    <div class="flex items-center">
      <img src="/path/to/logo.png" alt="Logo" class="h-8 w-auto" />
      <input
        type="text"
        placeholder="Search for collections, NFTs or users"
        class="ml-4 py-2 px-3 rounded-md bg-gray-800 text-white w-96"
      />
    </div>
    <nav class="space-x-4">
      <a href="#" class="text-white">Explore</a>
      <a href="#" class="text-white">How it works</a>
      <a href="#" class="text-white">About</a>
    </nav>
    <div>
      <button
        class="text-white bg-blue-500 hover:bg-blue-600 py-2 px-4 rounded"
      >
        Sign Up
      </button>
      <button
        class="text-white bg-gray-800 hover:bg-gray-700 py-2 px-4 rounded ml-2"
      >
        Sign In
      </button>
    </div>
  </header>
</template>

<script></script>

<style lang="scss" scoped></style>
