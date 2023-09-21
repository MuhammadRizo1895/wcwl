<template>
  <header class="header mt-5 px-3">
    <div
      class="header-content d-flex justify-content-between align-items-center"
    >
      <div class="header-content__img-box">
        <img
          src="./assets/images/logo-white.png"
          alt="CheryLogo"
          width="280px"
        />
        <img src="./assets/images/wcwl.svg" alt="WCWL" width="300px" />
      </div>
      <div
        class="header-content__location d-flex align-items-center justify-content-end"
      >
        <p class="fs-4 me-4"><i class="fas fa-location-dot me-2"></i>Ташкент</p>
      </div>
    </div>
  </header>
  <div class="section px-3 my-5 d-flex align-items-center">
    <div class="section-content w-50">
      <h1 class="h-info lh-md">
        Закрытый клуб владельцев Сhery. Станьте частью чего-то большего
      </h1>
    </div>
    <div
      class="section-img-box w-50 d-flex justify-content-end align-items-center"
    >
      <Carusel class="ms-auto" />
    </div>
  </div>
  <div class="section-club px-3 my-5">
    <h1 class="my-3">Наши клубы</h1>
    <div class="section-club__content d-flex align-items-center">
      <ClubBox v-for="club in clubs" :club="club" :key="club.clubName" />
    </div>
    <hr class="border border-danger border-4 rounded opacity-75" />
  </div>
  <div class="section-community px-3 my-5">
    <h1 class="w-50">
      Станьте частью дружелюбного комьюнити Chery и будьте в курсе всех новостей
      и мероприятий в вашем городе
    </h1>
    <div class="section-community-items my-5">
      <Community />
    </div>
  </div>
  <div class="my-5 section-img">
      <p>Присоединяйтесь к нам.</p>
    </div>
  <div
      class="section-images row no-gutters img-container my-5 rounded-bottom-5 py-3 w-100 mx-0"
    >
      <ImageBox />
      <!-- <Pagination/> -->
    </div>
  <!-- <div class="mt-5 py-5">
      <Representation />
    </div> -->
  <!-- <FooterItem /> -->
</template>
<script>
import Carusel from "../src/components/Carusel.vue";
import ClubBox from "../src/components/ClubBox.vue";
import Community from "./components/Community.vue";
import ImageBox from "./components/ImageBox.vue";
import Representation from "./components/Representation.vue";
import FooterItem from "./components/FooterItem.vue";
// import Pagination from "./components/Pagination.vue";
export default {
  components: {
    Carusel,
    ClubBox,
    Community,
    ImageBox,
    Representation,
    FooterItem,
    // Pagination,
  },
  data() {
    return {
      clubs: [
        {
          clubName: "Chery Tiggo 8 pro max Club",
          address: "Tashkent",
          social: {
            instagram: {
              nameSocial: "Instagram",
              classIcon: "fa-instagram",
              socialLink: "#",
            },
            telegram: {
              nameSocial: "Telegram",
              classIcon: "fa-telegram",
              socialLink: "#",
            },
            facebook: {
              nameSocial: "Facebook",
              classIcon: "fa-facebook",
              socialLink: "#",
            },
          },
          followers: 876,
        },
        {
          clubName: "Chery Tiggo 8 pro max Club",
          address: "Tashkent",
          social: {
            instagram: {
              nameSocial: "Instagram",
              classIcon: "fa-instagram",
              socialLink: "#",
            },
            telegram: {
              nameSocial: "Telegram",
              classIcon: "fa-telegram",
              socialLink: "#",
            },
            facebook: {
              nameSocial: "Facebook",
              classIcon: "fa-facebook",
              socialLink: "#",
            },
          },
          followers: 896,
        },
        {
          clubName: "Chery Tiggo 8 pro max Club",
          address: "Tashkent",
          social: {
            instagram: {
              nameSocial: "Instagram",
              classIcon: "fa-instagram",
              socialLink: "#",
            },
            telegram: {
              nameSocial: "Telegram",
              classIcon: "fa-telegram",
              socialLink: "#",
            },
            facebook: {
              nameSocial: "Facebook",
              classIcon: "fa-facebook",
              socialLink: "#",
            },
          },
          followers: 86,
        },
      ],
    };
  },
};
</script>
<style lang="scss">
$mobile: 360px;

@media (max-width: $mobile) {
  .header {
    margin-top: 10px !important;
    .header-content__img-box {
      display: flex;
      flex-direction: column;
      img {
        width: 120px;
        margin-top: 10px;
      }
    }
    .header-content__location {
      p {
        font-size: 16px !important;
      }
    }
  }
  .section {
    display: block !important;
    margin-top: 30px !important;
    .section-content {
      width: 100% !important;
      h1 {
        font-size: 20px;
        text-align: center;
      }
    }
    .section-img-box {
      width: 100% !important;
      margin-top: 20px;
    }
  }
  .section-club {
    h1 {
      font-size: 20px;
      text-align: center;
    }
    .section-club__content {
      flex-direction: column !important;
      .club-box {
        width: 100%;
      }
    }
  }
  .section-community {
    h1 {
      width: 100% !important;
      font-size: 20px;
      margin-right: 0px !important;
      text-align: center;
    }
    .section-community-items {
      .community-box .wrapper {
        height: 100px !important;
        align-items: center;
        .icon-box {
          width: 50px;
          height: 50px;
          font-size: 20px;
        }
        .info-box {
          width: 60%;
          padding: 10px;
          line-height: 1;
          font-size: 16px;
        }
        .num {
          font-size: 50px;
          display: flex;
          align-items: center;
          justify-content: center;
          width: 25%;
          color: #252528;
        }
      }
    }
  }
  .section-img{
    p{
      font-size: 20px;
    }
  }
}

.section-club {
  margin-top: 150px;
}
.h-info {
  font-size: 72px;
}
.section-img {
  width: 100%;
  height: 400px;
  background-image: url("/src/assets/images/tiggo8promax.jpg");
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-position: center;
  opacity: 0.2;
  font-size: 100px;
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 1;
}
.section-img p {
  color: #fff;
  z-index: 2;
}
.row.no-gutters {
  --bs-gutter-x: 0rem !important;
}
.img-container {
  background-color: #252528;
}
</style>
