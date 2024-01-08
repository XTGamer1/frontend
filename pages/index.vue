<script setup>
import { useRouter } from 'vue-router';

const router = useRouter();

useSeoMeta({
  ogTitle: "Home",
  ogDescription: "amvstrm - A streaming service for weebo...",
  ogUrl: useRoute().fullPath,
  twitterTitle: "Home",
  twitterDescription: "Animixwatch - A streaming service for weebo...",
  twitterCard: "summary",
});

useHead({
  htmlAttrs: {
    lang: "en",
  },
  title: "Home",
});

// Check if the route is the root path and redirect to '/pwa'
if (router.currentRoute.value.path === '/') {
  router.replace('/pwa');
}
</script>

<template>
  <PgCompsLandingPage />
</template> 

<style></style>
