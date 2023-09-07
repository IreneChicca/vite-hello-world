<script>
export default {
  data() {
    return {
      img: "heero.jpg",
    };
  },

  methods: {
    pathImg(img) {
      const imgUrl = new URL("../assets/img/" + img, import.meta.url);

      return imgUrl.href;
    },
  },
};
</script>

<template>
  <img :src="pathImg(img)" alt="" />
</template>

<style></style>
