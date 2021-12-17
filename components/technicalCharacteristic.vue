<template>
  <div class = '_container' ref = 'main'>
    <img :src="resolve_img_url(svgPath)">
    <div class = 'tech-title' ref = 'title'>{{title}}</div>
    <div class = 'tech-description' ref = 'desc'>{{description}}</div>
  </div>
</template>

<script>

export default {
  data() {
    return {

    }
  },
  props : ['title', 'description', 'svgPath', 'titleW'],
  methods : {
    resolve_img_url: function (path) {
      let images = require.context('../static/', false, /\.png$|\.jpg$|\.svg$/)
      return images("./"+path)
    }
  },
  mounted() {
    if (this.titleW) {
        this.$refs.title.style.width = this.titleW + 'px'
    }
  }
}

</script>

<style scoped>

._container {
  /*height : 222px;*/
  width : 211px;
  /*display : inline;*/
}

.tech-title {
  width: 183px;
  height: 54px;
  position: relative;
  top : 35.5px;

  font-family: Open Sans,serif;
  font-style: normal;
  font-weight: 600;
  font-size: 18px;
  line-height: 150%;

  text-align: center;
  color: #000000;
}

.tech-description {
  position : relative;
  top : 50px;
  width: 211px;
  height: 42px;

  font-family: Open Sans,serif;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 150%;

  text-align: center;
  color: #000000;
}


</style>
