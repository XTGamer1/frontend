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

// Check if the route is the root path and the device width is smaller than a certain threshold (e.g., 768px for common mobile devices)
if (router.currentRoute.value.path === '/' && isMobileWidth()) {
  router.replace('/pwa');
}

function isMobileWidth() {
  return window.innerWidth < 768; // Adjust the threshold as needed
}
</script>

<template>
  <PgCompsLandingPage />
</template> 

<style></style>
