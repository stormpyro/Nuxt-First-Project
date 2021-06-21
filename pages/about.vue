<template>
  <div>
    <h1>About us</h1>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus
      laudantium explicabo quisquam, similique cupiditate nemo asperiores
      veritatis nesciunt natus! Ratione optio culpa quod excepturi quam saepe
      facilis accusantium, eveniet minima?
    </p>
  </div>
</template>
<script>
export default {
  head: () => ({
    title: "Posts | About",
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