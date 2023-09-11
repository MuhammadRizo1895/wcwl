<template>
  <div class="carousel-item active text-white position-relative">
    <img :src="item.img" class="d-block w-100 " alt="img" />
    <div class="carousel-caption d-none d-md-block position-absolute bottom-0 p-0 text-end">
      <div class="py-2 px-2 bg-light text-dark w-50 mx-auto rounded-top-3">
        <div class="d-flex align-items-center justify-content-around">
          <img :src="item.icon" alt="icon" class="w-25" />
          <p>{{ item.title }}</p>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    item: {
      type: Object,
      required: true,
    },
  },
};
</script>
<style scoped>
</style>
