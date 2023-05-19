<template>
  <div>
    <HeaderArea />

    <slot />

    <FooterArea />
  </div>
</template>

<script setup>
import HeaderArea from "./HeaderArea";
import FooterArea from "./FooterArea";
</script>
