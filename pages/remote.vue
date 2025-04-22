<script setup>
import { defineAsyncComponent } from 'vue';

const RemoteComponent = defineAsyncComponent(() =>
  import('@/components/RemoteComponent.vue')
);
</script>

<template>
  <div>
    <h1>Remote Route in /remote</h1>
    <p>This page will load Remote Component below</p>
    <RemoteComponent />
    <p>source code is in <a href="https://github.com/jarooda/nuxt-layer-poc/tree/main">https://github.com/jarooda/nuxt-layer-poc/tree/main</a></p>
  </div>
</template>