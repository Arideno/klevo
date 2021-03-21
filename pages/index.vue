<template>
  <div class="container">
    <div class="row">
      <div class="col-12">
        <h1 class="title">Магазин майбутнього</h1>
      </div>
    </div>
    <div class="row">
      <div class="col-12 d-flex justify-content-center">
        <img class="w-100" src="~/assets/main_1.png" alt="Main">
      </div>
    </div>
    <div class="row grid-block">
      <div class="col-12 col-xl-6 d-flex justify-content-center">
        <div>
          <div class="grid-block__title">
            <p>В нас найкращий брендовий</p>
            <p>одяг з України та Європи</p>
          </div>
          <img src="~/assets/grid_1_1.png" alt="Grid11">
        </div>
      </div>
      <div class="col-12 col-xl-6 d-flex justify-content-center">
        <div>
          <div class="grid-block__title">
            <p>Ми підбераємо найкращі стилі</p>
            <p>для Ваших дітей</p>
          </div>
          <div class="grid-block__images">
            <img src="~/assets/grid_2_1.png" alt="Grid21">
            <img src="~/assets/grid_2_2.png" alt="Grid22">
            <img src="~/assets/grid_2_3.png" alt="Grid23">
            <img src="~/assets/grid_2_4.png" alt="Grid24">
          </div>
        </div>
      </div>
    </div>
    <div class="row images-block">
      <div class="col-12 d-flex justify-content-center">
        <h2 class="images-block__title">Ми даруємо радість Вам і Вашим дітям</h2>
      </div>
      <div class="col-12 images-block__images">
        <div class="d-flex justify-content-center">
          <img src="~/assets/main_2.png" alt="Main2">
        </div>
        <div class="d-flex justify-content-center two-images">
          <img src="~/assets/main_3.png" alt="Main3">
          <img src="~/assets/main_4.png" alt="Main4">
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-12">
        <h1 class="comment-title">Відгуки наших клієнтів</h1>
      </div>
    </div>
    <div class="row">
      <div
        class="col-12 comments-block d-flex flex-column flex-lg-row align-items-center justify-content-center ms-4 ms-lg-0">
        <Comment class="comment mb-5 mb-lg-0" img="bubble1.svg" name="Олена"
                 comment="Найкращий дитячий магазин у нашому місті!" :stars="5"/>
        <Comment class="comment mb-5 mb-lg-0" img="bubble2.svg" name="Дарія"
                 comment="Стільки емоцій))) Дуже привітний персонал" :stars="5"/>
        <Comment class="comment" img="bubble3.svg" name="Денис" comment="Гарний магазин" :stars="4"/>
      </div>
    </div>
    <div class="row">
      <div class="col-12">
        <h1 class="location-title">Де нас знайти</h1>
      </div>
    </div>
    <div class="row flex-column-reverse flex-lg-row contacts">
      <div class="col-12 d-block d-lg-none">
        <div class="contact-block">
          <div class="social-block">
            <div class="d-flex justify-content-center">
              <p class="mb-1">Ми у соціальних мережах</p>
            </div>
            <div class="d-flex mb-1">
              <img src="~/assets/instagram.svg" alt="Instagram">
              <p class="social-tag">@klevolook</p>
            </div>
            <div class="d-flex">
              <img src="~/assets/facebook.svg" alt="Facebook">
              <p class="social-tag">@klevo2017</p>
            </div>
          </div>
        </div>
      </div>
      <div class="col-12 col-lg-6 d-flex justify-content-center justify-content-lg-end mt-4 mt-lg-0">
        <iframe id="map" loading="lazy" allowfullscreen
                src="https://www.google.com/maps/embed/v1/place?q=place_id:Ej1Tb2Jvcm5hIFN0LCAxMywgTXlrb2xhaXYsIE15a29sYWl2cydrYSBvYmxhc3QsIFVrcmFpbmUsIDU0MDAwIlASTgo0CjIJWQGog2bJxUARMDj9Twa28tkaHgsQ7sHuoQEaFAoSCdUTcvuJy8VAETzhoXQKgl_IDBANKhQKEgkvvsmwesnFQBGm7fvu1AHIHQ&key=AIzaSyDf0gcNSSu8B5NxMzm3qzDoSFiZZ2SJW9A"></iframe>
      </div>
      <div class="col-12 col-lg-6 d-flex justify-content-center justify-content-lg-start">
        <div class="contact-block">
          <p class="text-center text-lg-start">Місто Миколаїв, вулиця Соборна 13/1</p>
          <p class="text-center text-lg-start mt-3 mt-lg-0">Телефон: +380 050 100 0175</p>
          <div class="social-block d-none d-lg-block">
            <p class="mb-1">Ми у соціальних мережах</p>
            <div class="d-flex mb-1">
              <img src="~/assets/instagram.svg" alt="Instagram">
              <p class="social-tag">@klevolook</p>
            </div>
            <div class="d-flex">
              <img src="~/assets/facebook.svg" alt="Facebook">
              <p class="social-tag">@klevo2017</p>
            </div>
          </div>
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

.grid-block {
  margin-top: 60px;
  margin-left: 95px;
  margin-right: 95px;

  .grid-block__title {
    color: $primary-color;
    font-size: 24px;
    text-align: center;
    margin-bottom: 20px;

    p {
      margin: 0;
    }
  }

  .grid-block__images {
    display: grid;
    grid-template-columns: 180px 180px;
    grid-template-rows: 180px 180px;
    grid-gap: 30px;
  }
}

.images-block {
  margin-top: 70px;

  .images-block__title {
    color: $secondary-color;
    font-size: 32px;
    text-align: center;
  }

  .images-block__images {
    margin-top: 25px;

    img {
      width: 100%;
    }

    .two-images {
      margin-top: 40px;

      img {
        &:first-child {
          margin-right: 40px;
        }
      }
    }
  }
}

.comment-title {
  color: $primary-color;
  font-size: 32px;
  text-align: center;
  margin-top: 80px;
  margin-bottom: 60px;
}

.comments-block {
  .comment {
    margin-right: 60px;

    :last-child {
      margin-right: 0;
    }
  }
}

.location-title {
  color: $secondary-color;
  font-size: 32px;
  text-align: center;
  margin-top: 75px;
  margin-bottom: 30px;
}

#map {
  width: 440px;
  height: 420px;
}

@media screen and (max-width: 960px) {
  #map {
    width: 100%;
  }
}

.contacts {
  margin-bottom: 30px;
}

.contact-block {
  font-family: 'Roboto', sans-serif;
  font-size: 18px;
  color: $grey-color;

  p {
    margin: 0;
  }

  .social-block {
    margin-top: 60px;

    .social-tag {
      margin-left: 10px;
      color: $secondary-color;
    }
  }
}

img {
  max-height: 100%;
}
</style>
