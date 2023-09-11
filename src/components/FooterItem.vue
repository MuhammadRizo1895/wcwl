<template>
  <footer>
    <div class="footer px-3">
      <div class="d-flex flex-column p-5 pt-0">
        <img src="../assets/images/wcwl.svg" alt="wcwl" />
      </div>
      <div class="d-flex">
        <div class="mx-4" style="width: 33%">
          <p class="fs-4">Горячая линия Chery</p>
          <p class="fs-1"><span class="text-danger">+998</span> 901234567</p>
          <br /><br />
          <p class="mb-3 text-secondary">
            &copy; 2023 АО &laquo;Roodell&raquo;
          </p>
        </div>
        <div class="d-flex flex-column" style="width: 33%">
          <div class="w-75">
            <p class="my-2 py-1 border-bottom border-white">
              <a class="text-white fs-5 text-decoration-none" href="#"
                >Правовая информация</a
              >
            </p>
            <p class="my-2 py-1 border-bottom border-white">
              <a class="text-white fs-5 text-decoration-none" href="#"
                >Спонсорам</a
              >
            </p>
          </div>
        </div>
        <div
          class="social-set d-flex align-items-center justify-content-center"
          style="width: 33%"
        >
          <div>
            <a href="#" class=" "><i class="fa-brands fa-facebook"></i></a>
            <a href="#" class=" "><i class="fa-brands fa-telegram"></i></a>
            <a href="#" class=" "><i class="fa-brands fa-instagram"></i></a>
            <a href="#" class=" "><i class="fa-brands fa-youtube"></i></a>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>
<script>
export default {};
</script>
<style>
.footer img {
  width: 600px;
}
.footer .social-set {
    text-align: center;
}
.footer .social-set a{
    padding: 15px;
    background-color: #fff;
    color: black;
    border-radius: 50%;
    font-size: 30px;
    margin: 0 10px;
}</style>
