<template>
  <div>

    <nav>
      <img src = '../static/navLogo.svg' class = 'navLogo'/>
      <div class = 'group-titles'>
        <span class = 'nav-title' style = 'margin-left : 0'>ORDER LENS</span>
        <span class = 'nav-title'>SHIPPING AND PAYMENT</span>
        <span class = 'nav-title'>COMPATIBILITY</span>
        <span class = 'nav-title'>RETURN POLICY</span>
        <span class = 'nav-title'>ABOUT US</span>
        <span class = 'nav-title' style = 'margin-right : 0'>NEWS</span>
      </div>
      <img src = '../static/navFacebook.svg' class = 'facebook'/>
    </nav>

    <div class = 'mainContainer'>
      <nuxt/>
    </div>

    <footer>


    </footer>

  </div>
</template>

<style scoped>

.facebook {
  position : absolute;
  right: 15.99%;
  top : 15px;
}

.navLogo {
  position : absolute;
  left: 15.99%;
  top : 13px;
}

.group-titles {
  /*width : 732px;*/
  position : relative;
  top : 16px;
  margin-left : auto;
  margin-right : auto;
  text-align : center;
}

.nav-title {
  font-family: Open Sans,serif;
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  line-height: 150%;
  margin-left: 30px;
  margin-right : 30px;
  /* or 21px */


  color: #FFFFFF;
}

</style>
