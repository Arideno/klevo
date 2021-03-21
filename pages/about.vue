<template>
  <div class="container">
    <div class="row">
      <div class="col-12">
        <h1 class="title">Контакти</h1>
      </div>
    </div>

    <div class="row mb-5 mt-5">
      <div class="col-lg-6 d-none d-lg-block">
        <h2 class="form-title">
          Якщо у вас є скарги, пропозиції або коментарі по роботі магазину - заповніть форму
        </h2>
        <div class="d-flex justify-content-center">
          <form class="contact-form">
            <div class="d-flex justify-content-center">
              <label>
                <input type="text" class="input-field" placeholder="Ім’я">
              </label>
            </div>
            <div class="d-flex justify-content-center">
              <label>
                <input type="email" class="input-field" placeholder="Email">
              </label>
            </div>
            <div class="d-flex justify-content-center">
              <label>
                <textarea class="text" placeholder="Текст"></textarea>
              </label>
            </div>
            <div class="d-flex justify-content-center">
              <button class="send">
                Відправити
              </button>
            </div>
          </form>
        </div>
      </div>
      <div class="col-12 col-lg-6">
        <h2 class="contact-title">
          Телефони
        </h2>
        <ul class="phones">
          <li><a href="tel:+380950000000">Vodaphone: +380950000000</a></li>
          <li><a href="tel:+380970000000">Kyivstart: +380970000000</a></li>
          <li><a href="tel:+380930000000">Lifecell: +380930000000</a></li>
        </ul>
        <div class="social-info">
          <h2 class="sm-title">
            Наші соціальні мережі
          </h2>
          <div class="socials">
            <a href="#"><img src="~/assets/instagram_blue.svg" alt="Instagram"></a>
            <a href="#"><img src="~/assets/facebook_blue.svg" alt="Facebook"></a>
            <a href="#"><img src="~/assets/youtube.svg" alt="Youtube"></a>
          </div>
        </div>
        <h2 class="address">Місто Миколаїв, вулиця Соборна 13/1</h2>
        <div class="d-flex justify-content-center">
          <iframe id="map" loading="lazy" allowfullscreen src="https://www.google.com/maps/embed/v1/place?q=place_id:Ej1Tb2Jvcm5hIFN0LCAxMywgTXlrb2xhaXYsIE15a29sYWl2cydrYSBvYmxhc3QsIFVrcmFpbmUsIDU0MDAwIlASTgo0CjIJWQGog2bJxUARMDj9Twa28tkaHgsQ7sHuoQEaFAoSCdUTcvuJy8VAETzhoXQKgl_IDBANKhQKEgkvvsmwesnFQBGm7fvu1AHIHQ&key=AIzaSyDf0gcNSSu8B5NxMzm3qzDoSFiZZ2SJW9A"></iframe>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.title {
  color: $secondary-color;
  text-align: center;
  font-size: 32px;
  margin-top: 40px;
}

.form-title {
  font-size: 24px;
  color: $primary-color;
  text-align: center;
}

form.contact-form {
  width: 382px;
  height: 606px;
  background-color: $secondary-color;
  border-radius: 40px;
  margin-top: 35px;

  input.input-field {
    width: 270px;
    height: 40px;
    background-color: #fff;
    border-radius: 20px;
    border: none;
    padding-left: 20px;
    outline: none;

    &::placeholder {
      color: #ADADAD;
      font-size: 18px;
    }

    &:first-child {
      margin-top: 40px;
    }

    &:last-child {
      margin-top: 50px;
    }
  }

  textarea.text {
    width: 270px;
    height: 217px;
    border-radius: 20px;
    border: none;
    padding-left: 20px;
    padding-top: 15px;
    margin-top: 50px;
    background-color: #fff;
    resize: none;
    outline: none;

    &::placeholder {
      color: #ADADAD;
      font-size: 18px;
    }
  }

  button.send {
    margin-top: 70px;
    width: 270px;
    height: 60px;
    background-color: $primary-color;
    border-radius: 20px;
    font-size: 24px;
    color: #fff;
    border: none;
  }
}

.contact-title {
  font-size: 24px;
  color: $primary-color;
  text-align: center;
}

ul.phones {
  margin-top: 45px;
  list-style: none;

  li {
    text-align: center;

    a {
      text-decoration: none;
      color: $secondary-color;
      font-size: 24px;
    }
  }
}

.sm-title {
  font-size: 24px;
  color: $primary-color;
  margin-top: 70px;
  text-align: center;
}

.social-info {
  margin-left: 20px;
}

.socials {
  margin-top: 20px;
  display: flex;
  justify-content: center;

  img {
    width: 35px;
    height: 35px;

    margin-right: 25px;

    :last-child {
      margin-right: 0;
    }
  }
}

.address {
  font-size: 14px;
  color: $primary-color;
  margin-top: 60px;
  text-align: center;
}

#map {
  margin-top: 20px;
  width: 469px;
  height: 292px;
}
</style>
