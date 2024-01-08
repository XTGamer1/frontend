<meta http-equiv="refresh" content="0;url=/pwa">

<script setup>
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
</script>

<template>
  <PgCompsLandingPage />
</template> 

<style></style>
