<template>
  <div v-for="(image, index) in CurrentImages" :key="index" class="col-md-4 col-sm-12 p-1">
    <div class="img-box rounded text-center py-3">
      <img :src="image" alt="img" width="420" class="rounded-4" />
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      CurrentImages: [
        "./src/assets/images/all/img1.jpg",
        "/src/assets/images/all/img2.jpg",
        "/src/assets/images/all/img3.jpg",
        "/src/assets/images/all/img4.jpg",
        "/src/assets/images/all/img5.jpg",
        "/src/assets/images/all/img6.jpg",
        "/src/assets/images/all/img7.jpg",
        "/src/assets/images/all/img8.jpg",
        "/src/assets/images/all/img9.jpg",
        "/src/assets/images/all/img10.jpg",
        "/src/assets/images/all/img11.jpg",
        "/src/assets/images/all/img12.jpg",
        "/src/assets/images/all/img13.jpg",
        "/src/assets/images/all/img14.jpg",
        "/src/assets/images/all/img15.jpg",
        "/src/assets/images/all/img16.jpg",
        "/src/assets/images/all/img17.jpg",
        "/src/assets/images/all/img18.jpg",
        "/src/assets/images/all/img19.jpg",
        // "/src/assets/images/all/img20.jpg",
        "/src/assets/images/all/img21.jpg",
      ],
    };
  },
};
</script>
<style></style>
