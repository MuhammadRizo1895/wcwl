<template>
  <div
    id="carouselExampleAutoplaying"
    class="carousel slide"
    data-bs-ride="carousel"
  >
    <div class="carousel-inner w-75 mx-auto rounded-4">
      <CaruselItem v-for="item in caruselData" :item="item" :key="item.id"/>
    </div>
  </div>
</template>
<script>
import CaruselItem from "./CaruselItem.vue";

export default {
  components: {
    CaruselItem,
  },
  data() {
    return {
      slide: 0,
      sliding: null,
      caruselData: [
        {
          id: 1,
          img: "/src/assets/images/party/img1.JPG",
          icon:"/src/assets/images/icon/giftbox.png",
          title: "подарки",
        },
        {
          id: 2,
          img: "/src/assets/images/party/img2.JPG",
          icon:"/src/assets/images/icon/loudspeaker.png",
          title: "живое общение",
        },
        {
          id: 3,
          img: "/src/assets/images/party/img3.JPG",
          icon:"/src/assets/images/icon/party-popper.png",
          title: "тусовки",
        },
        {
          id: 4,
          img: "/src/assets/images/party/img4.JPG",
          icon:"/src/assets/images/icon/light-bulb.png",
          title: "интересный",
        },
      ],
    };
  },
};
</script>
<style></style>
