<template>
  <div class="comment">
    <img class="bubble" :src="require(`~/assets/${img}`)" alt="Bubble">
    <h3 class="name">{{ name }}</h3>
    <img class="brackets" src="~/assets/brackets.svg" alt="Brackets">
    <p class="comment__text">{{ comment }}</p>
    <div class="stars">
      <div class="star filled" v-for="index in filledStarsArray" :key="index"></div>
      <div class="star" v-for="index in unfilledStarsArray" :key="index"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Comment",
  props: {
    img: String,
    name: String,
    comment: String,
    stars: Number
  },
  computed: {
    filledStarsArray() {
      let foo = []
      for (let i = 0; i < this.stars; i++) {
        foo.push(i)
      }
      return foo
    },
    unfilledStarsArray() {
      let foo = []
      for (let i = 0; i < 5 - this.stars; i++) {
        foo.push(i)
      }
      return foo
    }
  }
}
</script>

<style lang="scss" scoped>
.comment {
  display: block;
  width: 315px;
  height: 260px;
  position: relative;
}

.bubble {
  position: absolute;
  z-index: -1;
}

.name {
  font-size: 24px;
  color: #fff;
  position: absolute;
  left: 120px;
  top: 15px;
}

.brackets {
  position: absolute;
  left: 35px;
  top: 80px;
}

.comment__text {
  font-family: 'Roboto', sans-serif;
  font-weight: 400;
  font-style: italic;
  color: #fff;
  position: absolute;
  top: 120px;
  left: 30px;
  right: 30px;
  text-align: center;
  line-height: 20px;
}

.stars {
  display: flex;
  position: absolute;
  top: 170px;
  left: 80px;
  justify-content: center;

  .star {
    background-image: url("~/assets/star_unfilled.svg");
    width: 25px;
    height: 25px;
    margin-right: 10px;

    :last-child {
      margin-right: 0;
    }

    &.filled {
      background-image: url("~/assets/star_filled.svg");
    }
  }
}
</style>
