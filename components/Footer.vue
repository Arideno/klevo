<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-3">
        <div class="logo-block">
          <div class="d-flex justify-content-center">
            <img class="logo" src="~/assets/logo_2.svg" alt="Klevo">
          </div>
          <div class="d-flex justify-content-center">
            <div class="copy">
              <p>Copyright &copy; 2017-2021 Klevo.</p>
              <p>All rights reserved.</p>
            </div>
          </div>
        </div>
      </div>
      <div class="col-6 d-flex">
        <div class="links">
          <h2>Компанія</h2>
          <ul>
            <li><a href="#">Про нас</a></li>
            <li><a href="#">Контакти</a></li>
            <li><a href="#">Вакансії</a></li>
          </ul>
        </div>
        <div class="links">
          <h2>Інформація</h2>
          <ul>
            <li><a href="#">Питання та відповіді</a></li>
            <li><a href="#">Новини</a></li>
            <li><a href="#">Акції</a></li>
          </ul>
        </div>
        <div class="links">
          <h2>Популярні категорії</h2>
          <ul>
            <li><a href="#">Одяг</a></li>
            <li><a href="#">Іграшки</a></li>
            <li><a href="#">Товари для мам</a></li>
          </ul>
        </div>
      </div>
      <div class="col-3">
        <div class="d-flex justify-content-end">
          <div class="info">
            <p>м. Миколаїв, вул Соборна 13/1</p>
            <p>Телефон: +380 050 100 0175</p>
          </div>
        </div>
        <div class="contact-buttons">
          <div class="question-button">
            <p>Задати питання</p>
          </div>
          <img src="~/assets/instagram_white.svg" alt="Instagram">
          <img src="~/assets/facebook_white.svg" alt="Facebook">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer"
}
</script>

<style lang="scss" scoped>
.container-fluid {
  background-color: $secondary-color;
  height: 140px;
}

.logo-block {
  height: 140px;
  position: relative;
}

.logo {
  position: absolute;
  top: -40px;
  left: auto;
}

.copy {
  font-size: 12px;
  color: #fff;
  position: absolute;
  bottom: 10px;

  p {
    margin: 0;
    text-align: center;
  }
}

.links {
  color: #fff;
  margin-top: 15px;
  margin-right: 50px;

  &:last-child {
    margin-right: 0;
  }

  h2 {
    font-size: 18px;
  }

  ul {
    font-size: 14px;
    list-style: none;
    padding: 0;

    a {
      color: #fff;
      text-decoration: none;
    }
  }
}

.info {
  font-size: 13px;
  color: #fff;
  margin-top: 35px;
  margin-right: 45px;

  p {
    margin: 0;
    text-align: right;
  }
}

.contact-buttons {
  display: flex;
  margin-top: 20px;
  justify-content: end;
  margin-right: 45px;

  img {
    width: 35px;
    height: 35px;

    margin-right: 15px;

    &:last-child {
      margin-right: 0;
    }
  }

  .question-button {
    width: 120px;
    height: 30px;
    background-color: $primary-color;
    border-radius: 15px;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-right: 35px;

    p {
      color: #fff;
      font-size: 12px;
      margin: 0;
    }
  }
}
</style>
