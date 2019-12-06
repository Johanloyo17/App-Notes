<template>
  <div>
    <NavBar/>
      <router-view></router-view>
  </div>
</template>

<script>
  import NavBar from'../components/NavBar'
  export default {
    components: {
      NavBar
    },
  }
</script>


<style lang="stylus">
  @import'../Stylus/main.styl'
  @font-face {
    font-family: bebas;
    src: url(../assets/BebasNeue-Regular.ttf);
    src: url(../assets/BebasNeue-Regular.otf);
  }
  @font-face {
    font-family: sf;
    src: url(../assets/SFProDisplay-Regular.ttf);
  }
  @font-face {
    font-family: myriad;
    src: url(../assets/MYRIADPRO-REGULAR.ttf);
  }
  @font-face {
    font-family: myriad-bold;
    src: url(../assets/MYRIADPRO-BOLD.ttf);
  }

</style>