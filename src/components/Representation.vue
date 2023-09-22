<template>
  <div class="representation-content d-flex">
    <div class="representation px-5">
      <h2>Хотите стать представителем Chery?</h2>
      <br /><br />
      <h2>Принимайте участие в программе лояльности Chery!</h2>
      <br /><br />
      <div>
        <h2>Условия простые:</h2>
        <h2>1) вы - владелец Chery,</h2>
        <h2>2) вы активно ведете социальные сети.</h2>
      </div>
      <br /><br />
      <h2>Заполняйте анкету, мы свяжемся с вами и расскажем подробнее.</h2>
    </div>
    <div class="form-representation">
      <form action="#">
        <div class="input-wrapper  my-5">
          <div class="input-box p-0">
            <label id="name" for="exampleFormControlInput1" class="form-label"
              >Как к вам обращаться?*
            </label>
            <input
              name="name"
              type="text"
              class="form-control"
              placeholder="Имя Фамилия"
              aria-label="Имя Фамилия"
            />
          </div>
          <div class="input-box p-0">
            <label id="tel" for="exampleFormControlInput1" class="form-label"
              >Укажите ваш номер телефона*
            </label>
            <input
              name="tel"
              type="tel"
              class="form-control"
              placeholder="Номер телефона"
              aria-label="Номер телефона"
            />
          </div>
        </div>
        <div class="input-wrapper  my-5">
          <div class="input-box p-0">
            <label id="email" for="exampleFormControlInput1" class="form-label"
              >Укажите Ваш E-mail*
            </label>
            <input
              type="email"
              class="form-control"
              placeholder="Ваш Е-mail"
              aria-label="Ваш Е-mail"
            />
          </div>
          <div class="input-box p-0">
            <label for="exampleFormControlInput1" class="form-label"
              >Город проживания*
            </label>
            <input
              type="text"
              class="form-control"
              placeholder="Город"
              aria-label="Город"
            />
          </div>
        </div>
        <div class="input-wrapper my-5">
          <div class="input-box p-0">
            <label id="model" for="exampleFormControlInput1" class="form-label"
              >Какая у вас модель автомобиля?*
            </label>
            <input
              name="model"
              type="text"
              class="form-control"
              placeholder="Model"
              aria-label="Model"
            />
          </div>
          <div class="input-box p-0">
            <label id="car" for="exampleFormControlInput1" class="form-label"
              >Укажи, пожалуйста, VIN**
            </label>
            <input
              name="car"
              type="text"
              class="form-control"
              placeholder="VIN  Автомобиля"
              aria-label="VIN  Автомобиля"
            />
          </div>
        </div>
        <div class="input-wrapper my-5">
          <div class="submit-wrapper">
            <input type="checkbox" name="conditions" id="conditions" /><br />
            <p>
              Я согласен с <br /><a href="#" class="conditions"
                >условиями обработки персональных данных</a
              >
            </p>
            <button type="submit" class="btn my-3 rounded-pill py-3 px-4">
              Отправить заявку
            </button>
          </div>
        </div>
      </form>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style>
.representation {
  width: 65%;
}
.representation h2 {
  font-size: 42px;
  margin-bottom: 12px;
}
.form-representation {
  height: 800px;
  width: 35%;
}
.form-representation .row {
  /* width: 90%; */
}
.form-representation .input-box {
  height: 100px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.input-box input {
  width: 75%;
  background: #171719;
  border: none;
  outline: none;
  border-bottom: 2px solid #a6192e;
  border-radius: 0;
}
.input-box input:focus {
  background-color: #171719;
  outline: none;
  box-shadow: none;
  border: none;
  border-bottom: 2px solid #a6192e;
  color: #fff;
}
.input-box input::placeholder {
  color: #8b8686;
}
.form-representation input[type="checkbox"] {
  width: 25px;
  height: 25px;
}
.form-representation input[type="checkbox"]:checked {
  width: 25px;
  height: 25px;
  accent-color: #a6192e !important;
}
.form-representation .conditions {
  color: #8b8686;
}
.form-representation button[type="submit"] {
  background-color: #a6192e;
  color: #fff;
  font-size: 20px;
}
</style>
