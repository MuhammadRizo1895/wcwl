<template>
  <div class="club-box">
    <div class="box p-4 position-relative">
      <h2 class="my-2">{{ club.clubName }}</h2>
      <p class="fs-5">
        <i class="fa-solid fa-location-dot me-2"></i>{{ club.address }}
      </p>
      <template v-for="social in club.social" :key="social.nameSocial">
        <p class="my-1">
          <i class="fa-brands me-2" :class="social.classIcon"></i
          >{{ social.nameSocial }}
        </p>
      </template>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    club: {
      type: Object,
      required: true,
    },
  },
};
</script>
<style scoped>
.club-box {
  width: 33.33%;
  height: 300px;
  padding: 15px;
}
.club-box .box {
  width: 90%;
  height: 250px;
  margin: 0 auto;
  border-radius: 20px;
  background-color: #252528;
}
.club-box .box:hover {
  background-color: #3d3d42;
  /* background-color: #A6192E; */
}
.followers {
  font-size: 75px;
  color: #4f4f52;
  top: 140px;
  left: 160px;
}
</style>
