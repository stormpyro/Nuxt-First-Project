<template>
  <h1>Welcome to my first nuxt app</h1>
</template>
<script>
export default {
  head: () => ({
    title: "Application Nuxt Posts | Home",
    meta: [
      {
        hid: "description",
        name: "description",
        content: "Website about posts",
      },
    ],
    htmlAttrs: {
      lang: "en",
    },
  }),
};
</script>

