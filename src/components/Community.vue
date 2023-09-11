<template>
  <div class="community-box w-100 h-25 border-1 border-danger">
    <div v-for="item in community" :item="item" :key="item.title" class="wrapper d-flex">
      <div class="icon-box">
        <i :class="item.icon"></i>
      </div>
      <div class="info-box">{{ item.title }}</div>
      <div class="num">{{ item.num }}</div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      community: [
        {
          icon: "fa-regular fa-comment",
          title:
            "Общайтесь с владельцами Chery",
          num: "01",
        },
        {
          icon: "fa-solid fa-rss",
          title:
            "Узнавайте первым новости и спецпредложения",
          num: "02",
        },
        {
          icon: "fa-solid fa-house-lock",
          title:
            "Участвуйте в закрытых мероприятиях в вашем городе",
          num: "01",
        },
      ],
    };
  },
};
</script>
<style scoped>
.wrapper {
  width: 100%;
  height: 200px;
  margin-bottom: 50px;
}
.wrapper .icon-box {
  width: 200px;
  height: 200px;
  border-radius: 50% 50% 50% 0;
  background-color: #a6192e;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 50px;
}
.wrapper .info-box {
  width: 60%;
  padding: 10px 16px;
  line-height: 2;
  font-size: 28px;
}
.wrapper .num {
  font-size: 180px;
  display: flex;
  align-items: center;
  justify-content: center;
  width: 25%;
  color: #252528;
}
</style>
