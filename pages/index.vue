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

// Check if the route is the root path and the device is a mobile device
if (shouldRedirect()) {
  router.replace('/pwa');
}

function shouldRedirect() {
  // Customize this condition based on your requirements
  return window.innerWidth < 768 && /Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(navigator.userAgent);
}
</script>

<template>
  <PgCompsLandingPage />
</template> 

<style></style>
