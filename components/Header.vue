<template>
  <div class="container-fluid">
    <div class="row h-100">
      <div class="d-flex d-xl-none col-12 justify-content-between align-items-center">
        <img class="call-img" src="~/assets/phone-call.svg" alt="Call">
        <img src="~/assets/logo_1.svg" alt="Klevo">
        <img class="list-img" src="~/assets/list.svg" alt="Menu>">
      </div>
      <div class="d-none d-xl-block col-xl-7">
        <img src="~/assets/logo_1.svg" alt="Klevo">
        <ul class="links">
          <li class="link-item">
            <NuxtLink to="/">Головна</NuxtLink>
          </li>
          <li class="link-item">
            <a href="#">Галерея</a>
          </li>
          <li class="link-item">
            <a href="#">Новини</a>
          </li>
          <li class="link-item">
            <a href="#">Магазин</a>
          </li>
          <li class="link-item">
            <NuxtLink to="/about">Контакти</NuxtLink>
          </li>
        </ul>
      </div>
      <div class="d-none d-xl-flex col-xl-5 right-buttons">
        <a href="tel:+3800501000175" class="call-btn">
          <p class="call-btn-title">Зателефонувати</p>
          <p class="call-btn-number">+380 050 100 0175</p>
        </a>
        <div class="address-block">
          <p>м. Миколаїв</p>
          <p>вул. Соборна 13/1</p>
        </div>
        <div class="images">
          <img src="~/assets/loupe 1.svg" alt="Search">
          <img src="~/assets/user 1.svg" alt="Profile">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header"
}
</script>

<style lang="scss" scoped>
.container-fluid {
  left: 0;
  top: 0;
  background: #fff;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
  height: 80px;
  position: sticky;
  z-index: 10000;
}

.links {
  display: inline-flex;
  flex-direction: row;
  list-style: none;
  padding: 0;
  margin: auto 0;
}

.link-item {
  margin-right: 30px;

  :last-child {
    margin-right: 0;
  }
}

a {
  text-decoration: none;
  color: $grey-color;
  size: 20px;
  &.nuxt-link-exact-active {
    color: $primary-color;
  }
}

.call-img {
  width: 30px;
  height: 30px;
  margin-left: 20px;
}

.list-img {
  width: 30px;
  height: 30px;
  margin-right: 20px;
}

.right-buttons {
  display: flex;
  align-items: center;
  justify-content: flex-end;

  .call-btn {
    width: 120px;
    height: 50px;
    background-color: $primary-color;
    border-radius: 15px;
    padding-top: 8px;
  }

  .call-btn-title, .call-btn-number {
    color: #fff;
    font-size: 10px;
    text-align: center;
    margin: 0;
  }

  .call-btn-title {
    font-size: 12px;
  }

  .address-block {
    font-family: 'Roboto', sans-serif;
    font-weight: 500;
    color: $grey-color;
    margin-left: 30px;
    text-align: center;

    p {
      margin: 0;
    }
  }

  .images {
    margin-left: 30px;
    margin-right: 44px;

    :first-child {
      margin-right: 15px;
    }
  }
}
</style>
