<template>
  <div class="container">
    <div class="row">
      <div class="col-12">
        <h1 class="title">Магазин</h1>
      </div>
    </div>
    <div class="row mb-4">
      <div class="col-lg-4 d-none d-lg-block">
        <div class="filters-block">
          <h2 class="filter-title">Категорія</h2>
          <ul class="categories">
            <li>
              <label class="radio">
                <span class="radio__input">
                  <input type="radio" name="category">
                  <span class="radio__control"></span>
                </span>
                <span class="radio__label">Одяг</span>
                <span class="radio__sublabel">3000</span>
              </label>
            </li>
            <li>
              <label class="radio">
                <span class="radio__input">
                  <input type="radio" name="category">
                  <span class="radio__control"></span>
                </span>
                <span class="radio__label">Lego</span>
                <span class="radio__sublabel">1500</span>
              </label>
            </li>
            <li>
              <label class="radio">
                <span class="radio__input">
                  <input type="radio" name="category">
                  <span class="radio__control"></span>
                </span>
                <span class="radio__label">Гігієна</span>
                <span class="radio__sublabel">300</span>
              </label>
            </li>
          </ul>
          <h2 class="filter-title">Вік</h2>
          <ul class="ages">
            <li>
              <label class="radio">
                <span class="radio__input">
                  <input type="radio" name="age">
                  <span class="radio__control"></span>
                </span>
                <span class="radio__label">до року</span>
              </label>
            </li>
            <li>
              <label class="radio">
                <span class="radio__input">
                  <input type="radio" name="age">
                  <span class="radio__control"></span>
                </span>
                <span class="radio__label">рік - 2 роки</span>
              </label>
            </li>
            <li>
              <label class="radio">
                <span class="radio__input">
                  <input type="radio" name="age">
                  <span class="radio__control"></span>
                </span>
                <span class="radio__label">3 роки - 5 років</span>
              </label>
            </li>
            <li>
              <label class="radio">
                <span class="radio__input">
                  <input type="radio" name="age">
                  <span class="radio__control"></span>
                </span>
                <span class="radio__label">6 років - 9 років</span>
              </label>
            </li>
            <li>
              <label class="radio">
                <span class="radio__input">
                  <input type="radio" name="age">
                  <span class="radio__control"></span>
                </span>
                <span class="radio__label">10 років - 12 років</span>
              </label>
            </li>
            <li>
              <label class="radio">
                <span class="radio__input">
                  <input type="radio" name="age">
                  <span class="radio__control"></span>
                </span>
                <span class="radio__label">дорослий</span>
              </label>
            </li>
          </ul>
          <h2 class="filter-title">Стать</h2>
          <ul class="categories">
            <li>
              <label class="radio">
                <span class="radio__input">
                  <input type="radio" name="gender">
                  <span class="radio__control"></span>
                </span>
                <span class="radio__label">хлопчик</span>
                <span class="radio__sublabel">3000</span>
              </label>
            </li>
            <li>
              <label class="radio">
                <span class="radio__input">
                  <input type="radio" name="gender">
                  <span class="radio__control"></span>
                </span>
                <span class="radio__label">дівчинка</span>
                <span class="radio__sublabel">1500</span>
              </label>
            </li>
            <li>
              <label class="radio">
                <span class="radio__input">
                  <input type="radio" name="gender">
                  <span class="radio__control"></span>
                </span>
                <span class="radio__label">хлопчик/дівчинка</span>
                <span class="radio__sublabel">300</span>
              </label>
            </li>
          </ul>
          <h2 class="filter-title">Ціна</h2>
          <div class="price">
            <input type="text" class="price-box" value="0">
            <span>-</span>
            <input type="text" class="price-box" value="25000">
          </div>
        </div>
      </div>
      <div class="col-12 col-lg-8">
        <button class="closed_filters d-flex d-lg-none justify-content-center align-items-center">
          <img src="~/assets/filter.svg" alt="Filter">
          <span>Фільтри</span>
        </button>
        <ul class="filters d-none d-lg-flex">
          <li class="active">по замовчуванню</li>
          <li>по популярності</li>
          <li>По ціні</li>
          <li>Спочатку нові</li>
        </ul>
        <div class="products">
          <div class="product">
            <span class="discount">-14%</span>
            <img class="product__img" src="~/assets/product.png" alt="Product">
            <div>
              <div class="additional_info">
                <span>16 років</span>
                <span>ТМ LEGO</span>
              </div>
              <div class="d-flex justify-content-center">
                <h3 class="product__title">LEGO® Star Wars™ Імперський зоряний руйнівник 75252</h3>
              </div>
              <div class="prices">
                <p class="original_price crossed">24 999 грн.</p>
                <p class="discount_price">21 402 грн.</p>
              </div>
              <div class="buttons">
                <button class="buy">Придбати</button>
                <button class="like">
                  <img src="~/assets/heart.svg" alt="Like">
                </button>
              </div>
            </div>
          </div>
          <div class="product">
            <span class="discount">-14%</span>
            <img class="product__img" src="~/assets/product.png" alt="Product">
            <div>
              <div class="additional_info">
                <span>16 років</span>
                <span>ТМ LEGO</span>
              </div>
              <div class="d-flex justify-content-center">
                <h3 class="product__title">LEGO® Star Wars™ Імперський зоряний руйнівник 75252</h3>
              </div>
              <div class="prices">
                <p class="original_price crossed">24 999 грн.</p>
                <p class="discount_price">21 402 грн.</p>
              </div>
              <div class="buttons">
                <button class="buy">Придбати</button>
                <button class="like">
                  <img src="~/assets/heart.svg" alt="Like">
                </button>
              </div>
            </div>
          </div>
          <div class="product">
            <img class="product__img" src="~/assets/product.png" alt="Product">
            <div>
              <div class="additional_info">
                <span>16 років</span>
                <span>ТМ LEGO</span>
              </div>
              <div class="d-flex justify-content-center">
                <h3 class="product__title">LEGO® Star Wars™ Імперський зоряний руйнівник 75252</h3>
              </div>
              <div class="prices">
                <p class="original_price">24 999 грн.</p>
              </div>
              <div class="buttons">
                <button class="buy">Придбати</button>
                <button class="like">
                  <img src="~/assets/heart.svg" alt="Like">
                </button>
              </div>
            </div>
          </div>
          <div class="product">
            <img class="product__img" src="~/assets/product.png" alt="Product">
            <div>
            <div class="additional_info">
              <span>16 років</span>
              <span>ТМ LEGO</span>
            </div>
            <div class="d-flex justify-content-center">
              <h3 class="product__title">LEGO® Star Wars™ Імперський зоряний руйнівник 75252</h3>
            </div>
            <div class="prices">
              <p class="original_price">24 999 грн.</p>
            </div>
            <div class="buttons">
              <button class="buy">Придбати</button>
              <button class="like">
                <img src="~/assets/heart.svg" alt="Like">
              </button>
            </div>
            </div>
          </div>
          <div class="product">
            <img class="product__img" src="~/assets/product.png" alt="Product">
            <div>
            <div class="additional_info">
              <span>16 років</span>
              <span>ТМ LEGO</span>
            </div>
            <div class="d-flex justify-content-center">
              <h3 class="product__title">LEGO® Star Wars™ Імперський зоряний руйнівник 75252</h3>
            </div>
            <div class="prices">
              <p class="original_price">24 999 грн.</p>
            </div>
            <div class="buttons">
              <button class="buy">Придбати</button>
              <button class="like">
                <img src="~/assets/heart.svg" alt="Like">
              </button>
            </div>
            </div>
          </div>
          <div class="product">
            <img class="product__img" src="~/assets/product.png" alt="Product">
            <div>
            <div class="additional_info">
              <span>16 років</span>
              <span>ТМ LEGO</span>
            </div>
            <div class="d-flex justify-content-center">
              <h3 class="product__title">LEGO® Star Wars™ Імперський зоряний руйнівник 75252</h3>
            </div>
            <div class="prices">
              <p class="original_price">24 999 грн.</p>
            </div>
            <div class="buttons">
              <button class="buy">Придбати</button>
              <button class="like">
                <img src="~/assets/heart.svg" alt="Like">
              </button>
            </div>
            </div>
          </div>
          <div class="product">
            <img class="product__img" src="~/assets/product.png" alt="Product">
            <div>
            <div class="additional_info">
              <span>16 років</span>
              <span>ТМ LEGO</span>
            </div>
            <div class="d-flex justify-content-center">
              <h3 class="product__title">LEGO® Star Wars™ Імперський зоряний руйнівник 75252</h3>
            </div>
            <div class="prices">
              <p class="original_price">24 999 грн.</p>
            </div>
            <div class="buttons">
              <button class="buy">Придбати</button>
              <button class="like">
                <img src="~/assets/heart.svg" alt="Like">
              </button>
            </div>
            </div>
          </div>
          <div class="product">
            <img class="product__img" src="~/assets/product.png" alt="Product">
            <div>
            <div class="additional_info">
              <span>16 років</span>
              <span>ТМ LEGO</span>
            </div>
            <div class="d-flex justify-content-center">
              <h3 class="product__title">LEGO® Star Wars™ Імперський зоряний руйнівник 75252</h3>
            </div>
            <div class="prices">
              <p class="original_price">24 999 грн.</p>
            </div>
            <div class="buttons">
              <button class="buy">Придбати</button>
              <button class="like">
                <img src="~/assets/heart.svg" alt="Like">
              </button>
            </div>
            </div>
          </div>
          <div class="product">
            <img class="product__img" src="~/assets/product.png" alt="Product">
            <div>
            <div class="additional_info">
              <span>16 років</span>
              <span>ТМ LEGO</span>
            </div>
            <div class="d-flex justify-content-center">
              <h3 class="product__title">LEGO® Star Wars™ Імперський зоряний руйнівник 75252</h3>
            </div>
            <div class="prices">
              <p class="original_price">24 999 грн.</p>
            </div>
            <div class="buttons">
              <button class="buy">Придбати</button>
              <button class="like">
                <img src="~/assets/heart.svg" alt="Like">
              </button>
            </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="row mb-4">
      <div class="col-12 d-flex justify-content-center">
        <div class="pages">
          <span class="page active">1</span>
          <span class="page">2</span>
          <span class="page">3</span>
          <span class="page">4</span>
          <span class="page">5</span>
        </div>
        <img src="~/assets/right-arrow.svg" alt="Next">
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

.filters-block {
  border: 1px solid #A0A0A0;
  border-radius: 50px;
  width: 100%;
  height: 860px;
  padding-left: 40px;

  .filter-title {
    margin-top: 40px;
    font-size: 24px;
    color: $primary-color;
    text-transform: uppercase;
  }

  .categories {
    list-style: none;
    padding: 0;
    margin-top: 30px;

    li {
      margin-bottom: 15px;

      &:last-child {
        margin-bottom: 0;
      }
    }
  }

  .ages {
    list-style: none;
    padding: 0;
    margin-top: 50px;

    li {
      margin-bottom: 15px;

      &:last-child {
        margin-bottom: 0;
      }
    }
  }

  .radio {
    display: grid;
    grid-template-columns: min-content max-content min-content;
    color: $secondary-color;

    .radio__input {
      display: flex;
      margin-right: 20px;

      input {
        opacity: 0;
        width: 0;
        height: 0;

        &:checked + .radio__control {
          background: radial-gradient(currentcolor 50%, rgba(255, 0, 0, 0) 51%);
        }
      }
    }

    .radio__label {
      line-height: 1;
      font-size: 18px;
      margin-right: 10px;
    }

    .radio__sublabel {
      line-height: 2;
      font-size: 10px;
      color: #A6A6A6;
    }

    .radio__control {
      display: block;
      width: 20px;
      height: 20px;
      border-radius: 50%;
      border: 0.1em solid currentColor;
      transform: translateY(-0.05em);
    }
  }
}

.price {
  display: flex;
  margin-top: 15px;

  .price-box {
    width: 70px;
    height: 30px;
    background-color: $primary-color;
    color: #fff;
    text-align: center;
    font-size: 12px;
    border: none;
    border-radius: 10px;
    outline: none;
  }

  span {
    margin-left: 10px;
    margin-right: 10px;
  }
}

.filters {
  list-style: none;
  width: 100%;
  border-radius: 40px;
  border: 1px solid #A0A0A0;
  padding: 24px 0;
  justify-content: space-around;

  li {
    color: $grey-color;
    text-transform: uppercase;
    cursor: pointer;
    transition: 0.3s;

    &.active {
      color: $primary-color;
    }

    &:hover {
      color: $primary-color;
    }
  }
}

.products {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 425px 425px 425px;

  .product {
    border-radius: 40px;
    position: relative;

    &:hover {
      border: 2px solid $primary-color;

      .buttons {
        display: flex;
      }
    }

    .product__img {
      margin-top: 35px;
      margin-left: 25px;
      margin-right: 25px;
    }

    .additional_info {
      display: flex;
      margin-top: 15px;
      margin-left: 25px;

      span {
        font-size: 14px;
        color: #A5A5A5;

        &:first-child {
          margin-right: 20px;
        }
      }
    }

    .product__title {
      max-width: 210px;
      color: $grey-color;
      text-align: center;
      margin-top: 15px;
      font-size: 14px;
    }

    .discount {
      display: flex;
      justify-content: center;
      align-items: center;
      width: 60px;
      height: 30px;
      background-color: $secondary-color;
      border-radius: 40px;
      position: absolute;
      font-size: 14px;
      color: #fff;
      top: 18px;
      left: 18px;
    }

    .prices {
      display: flex;
      justify-content: space-between;
      padding: 0 25px;

      .original_price {
        &.crossed {
          text-decoration: line-through;
        }
        color: #000;
        font-size: 18px;
      }

      .discount_price {
        font-size: 18px;
        color: $primary-color;
      }
    }

    .buttons {
      padding: 0 25px;
      justify-content: space-between;
      display: none;

      .buy {
        width: 130px;
        height: 35px;
        background-color: $primary-color;
        border-radius: 40px;
        color: #fff;
        font-size: 14px;
        border: none;
      }

      .like {
        border: none;
        background-color: white;
      }
    }
  }
}

.pages {
  display: flex;
  justify-content: center;

  .page {
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 24px;
    color: $primary-color;
    margin-right: 20px;
    width: 50px;
    height: 50px;

    &.active {
      background-color: $secondary-color;
      border-radius: 25px;
      color: white;
    }
  }
}

.closed_filters {
  color: $primary-color;
  height: 50px;
  border-radius: 40px;
  border: none;
  width: 100%;
}

@media screen and (max-width: 1140px) {
  .products {
    display: flex;
    flex-direction: column;

    .product {
      display: flex;
      border: none;

      .buttons {
        display: flex;
        padding: 0;
      }

      &:hover {
        border: none;
      }

      .additional_info {
        margin-left: 0;
      }

      .product__title {
        text-align: left;
      }

      .prices {
        padding: 0;
        .original_price, .discount_price {
          font-size: 14px;
        }
      }
    }
  }

  .pages {
    .page {
      width: 35px;
      height: 35px;
      font-size: 14px;
    }
  }
}
</style>
