<template>
  <div class="container">
    <div class="row">
      <div class="col-12">
        <h1 class="title">Магазин майбутнього</h1>
      </div>
    </div>
    <div class="row">
      <div class="col-12 d-flex justify-content-center">
        <img src="~/assets/main_1.png" alt="Main">
      </div>
    </div>
    <div class="row grid-block">
      <div class="col-md-6 d-flex justify-content-center">
        <div>
          <div class="grid-block__title">
            <p>В нас найкращий брендовий</p>
            <p>одяг з України та Європи</p>
          </div>
          <img src="~/assets/grid_1_1.png" alt="Grid11">
        </div>
      </div>
      <div class="col-md-6 d-flex justify-content-center">
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
        <img src="~/assets/main_2.png" alt="Main2">
        <img src="~/assets/main_3.png" alt="Main3">
        <img src="~/assets/main_4.png" alt="Main4">
      </div>
    </div>
    <div class="row">
      <div class="col-12">
        <h1 class="comment-title">Відгуки наших клієнтів</h1>
      </div>
    </div>
    <div class="row">
      <div class="col-12 comments-block d-flex justify-content-center">
        <Comment class="comment" img="bubble1.svg" name="Олена" comment="Найкращий дитячий магазин у нашому місті!" :stars="5" />
        <Comment class="comment" img="bubble2.svg" name="Дарія" comment="Стільки емоцій))) Дуже привітний персонал" :stars="5" />
        <Comment class="comment" img="bubble3.svg" name="Денис" comment="Гарний магазин" :stars="4" />
      </div>
    </div>
    <div class="row">
      <div class="col-12">
        <h1 class="location-title">Де нас знайти</h1>
      </div>
    </div>
    <div class="row contacts">
      <div class="col-12 col-md-6 d-flex justify-content-center justify-content-md-end">
        <google-map :center="{ lat: 46.965407, lng: 31.987489 }" :zoom="15" id="map">
          <google-map-marker :position="{ lat: 46.965407, lng: 31.987489 }"></google-map-marker>
        </google-map>
      </div>
      <div class="col-12 col-md-6 contact-block">
        <p>Місто Миколаїв, вулиця Соборна 13/1</p>
        <p>Телефон: +380 050 100 0175</p>
        <div class="social-block">
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
</template>

<script>
export default {}
</script>

<style lang="scss">
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
    display: grid;
    justify-content: center;
    grid-template-rows: auto;
    grid-template-columns: 440px 440px;
    grid-template-areas:
      "one one"
      "two three";
    grid-column-gap: 40px;
    grid-row-gap: 40px;

    :first-child {
      grid-area: one;
    }

    :nth-child(2) {
      grid-area: two;
    }

    :last-child {
      grid-area: three;
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
</style>
