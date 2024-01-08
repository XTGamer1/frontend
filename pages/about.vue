<script setup>
useSeoMeta({
  ogTitle: "About",
  ogDescription: "About amvstrm...",
  ogImage: "logo.png",
  ogUrl: "[og:url]",
  twitterTitle: "About",
  twitterDescription: "About amvstrm...",
  twitterImage: "logo.png",
  twitterCard: "summary",
});

useHead({
  htmlAttrs: {
    lang: "en",
  },
  title: "About",
});
</script>
<template>
  <v-container>
    <div style="height: fit-content; display: grid; place-items: center">
      <div class="pa-5" style="background-color: #212121">
        <h1><img src="/logo.png" alt="loho" height="50" /></h1>
        <p>
          Welcome to Animixwatch.me, your ultimate destination for immersive anime experiences. Delve into a vast library that spans the spectrum of genres, offering everything from timeless classics to the latest releases. Our commitment to high-quality streaming ensures that you can enjoy your favorite series and movies with crisp visuals and clear audio. Navigate seamlessly through our user-friendly interface and discover personalized recommendations based on your preferences. Animixwatch.me is not just a streaming platform; it's a community hub where like-minded anime enthusiasts connect, share, and celebrate the rich tapestry of this captivating art form. Join us on this anime adventure and start streaming today at Animixwatch.me.
        </p>
        <div class="mt-2">

        </div>
        <div class="my-5">
          <h1>Donation</h1>
          We do not use ADs and rely on donation to keep the website running forever. 
          You can consider donating us to keep it alive! <br>
          <v-btn
            class="mt-4"
            color="yellow-darken-1"
            prepend-icon="mdi-cash"
            href="https://www.buymeacoffee.com/whitefireshoto"
          >
            Donation
          </v-btn>
        </div>
      </div>
    </div>
  </v-container>
</template>
