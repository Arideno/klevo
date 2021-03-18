<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-md-6">
        <img src="~/static/logo_1.svg" alt="Klevo">
        <ul class="links">
          <li class="link-item">
            <NuxtLink to="/">Головна</NuxtLink>
          </li>
          <li class="link-item">
<!--            <NuxtLink to="/gallery">Галерея</NuxtLink>-->
          </li>
          <li class="link-item">
<!--            <NuxtLink to="/news">Новини</NuxtLink>-->
          </li>
          <li class="link-item">
<!--            <NuxtLink to="/shop">Магазин</NuxtLink>-->
          </li>
          <li class="link-item">
<!--            <NuxtLink to="/contacts">Контакти</NuxtLink>-->
          </li>
        </ul>
      </div>
      <div class="col-md-6 right-buttons">
        <div class="call-btn">
          <p class="call-btn-title">Зателефонувати</p>
          <p class="call-btn-number">+380 050 100 0175</p>
        </div>
        <div class="address-block">
          <p>м. Миколаїв</p>
          <p>вул. Соборна 13/1</p>
        </div>
        <div class="images">
          <img src="~/static/loupe 1.svg" alt="Search">
          <img src="~/static/user 1.svg" alt="Profile">
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

.right-buttons {
  display: flex;
  align-items: center;
  justify-content: end;

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
