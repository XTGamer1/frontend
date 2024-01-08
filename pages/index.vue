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

// Add the following code for client-side redirection
if (window.location.href === "https://animixwatch.me/") {
  window.location.href = "https://animixwatch.me/pwa";
}
</script>

<template>
  <PgCompsLandingPage />
</template> 

<style></style>
