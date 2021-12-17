<template>

  <div class = 'main'>
    <img class = 'card-img' :src = "resolve_img_url(imgPath)"/>
    <span class = 'product-description'>{{ title }}</span>
    <span class = 'price'>{{ price }}</span>
    <button class = 'button-more'>
      <span class = 'button-text'>More about this item</span>
    </button>
  </div>

</template>

<script>

export default {
  data() {
    return {

    }
  },
  props : ['imgPath', 'title', 'price'],
  methods : {
    resolve_img_url: function (path) {
      let images = require.context('../static/', false, /\.png$|\.jpg$|\.svg$/)
      return images("./"+path)
    }
  }
}

</script>

<style scoped>

.main {
  width : 409px;
  height : 596px;
  text-align : left;
}

.card-img {
  width : 409px;
  height : 409px;
}

.product-description {
  display : block;
  font-family: Open Sans,serif;
  font-style: normal;
  font-weight: 600;
  font-size: 24px;
  line-height: 150%;
  color: #000000;
  margin-bottom : 20px;
}

.price {
  @apply product-description;
}

.button-more {
  border: 1px solid #000000;
  box-sizing: border-box;
  border-radius: 7px;
  transition : all .25s ease-in-out;

  @apply px-4 py-1;
}

.button-more .button-text {
  font-family: Open Sans,serif;
  font-style: normal;
  font-weight: bold;
  font-size: 18px;
  line-height: 150%;

  color: #000000;
  transition : all .25s ease-in-out;
}

.button-more:hover, .button-more:hover .button-text {
  color : white;
  transition : all .25s ease-in-out;

}
.button-more:hover {
  background : black;
}

</style>
