<template>
    <NuxtLink
      :href="href"
      :target="target"
    >
      <slot />
    </NuxtLink>
  </template>
  
  <script setup lang="ts">
  defineProps({
    href: {
      type: String,
      default: ''
    },
    target: {
      type: String,
      default: undefined,
      required: false
    }
  })
  </script>

  <style>
  .document-driven-page {
    a {
        color: inherit;
        text-decoration: none;
        border-bottom: solid 1px #27ff62;
        padding-bottom: 2px;
        transition: border .2s ease-in;

        &:hover {
            border-bottom: solid 4px #27ff62;
        }
    }
  }

</style>