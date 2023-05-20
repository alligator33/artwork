<template>
  <button
    :class="[
      'text-white py-2 px-4 rounded',
      {
        'bg-blue-500 hover:bg-blue-600': type === 'primary',
        'bg-gray-800 hover:bg-gray-700': type === 'secondary',
      },
    ]"
  >
    <slot></slot>
  </button>
</template>

<script setup>
// export default {
//   name: "Button",
//   props: {
//     type: {
//       type: String,
//       default: "primary",
//     },
//   },
// };
</script>

<style scoped>
/* Add any additional styling for the button component */
</style>
