<template>
  <div id="app">
    <NavigationMobileComp />
    <div class="content" :class="{'open' :showNav}">
      <div class="bar">
        <div id="navigation-icon" v-if="mobileView" @click="showNav = !showNav">
          <i class="fas fa-bars"></i>
        </div>
      <NavigationComponent v-if="!mobileView" />
      </div>
      <ContentComponentt />
    </div>
  </div>
</template>


<script>
import NavigationComponent from './components/MyNavigation.vue'
import ContentComponentt from './components/MyContent.vue'
import NavigationMobileComp from './components/NavigationMobile.vue'

export default {
  name: 'App',
  components:{
    NavigationComponent,
    ContentComponentt,
    NavigationMobileComp,
  },
  data: () => {
    return{
      mobileView: true,
      showNav: false
    }
  },
  methods:{
    handleView(){
      this.mobileView = window.innerWidth <= 425;
    }
  },
  created(){
    this.handleView(),
    window.addEventListener('resize', this.handleView);
  }  


}
</script>

<style>
  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    text-decoration: none;
  }
  body{
    width: 100%;
    height: 100vh;
    margin: 0;
    padding: 0;
    background-color: #00487c;
  }

  #app{
    position: relative;
    padding: 10px;
    overflow: hidden;
    width: calc(100% );
    height: calc(100vh - 20px);
  }
  .bar{
    display: flex;
    width: 100%;
  }
  .content{
    position: absolute;
    top: 10px;
    width: calc(100%);
    height: 100%;
    padding: 20px;
    background-color: #8EA4D2;
    transition: 1s transform cubic-bezier(0,.12,.17,1);
  }
  .open{
    transform: translateX(100px);
  }

</style>
