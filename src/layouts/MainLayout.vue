<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated class="bg-white text-grey-10" bordered >
      <q-toolbar class="constrain">
         <q-btn 
         class = "large-screen-only q-mr-sm"
          to =  "/camera"
          icon="eva-camera-outline" size="18px"  flat round dense/>

          <q-separator vertical spaced  class="large-screen-only"/>
        <q-toolbar-title class="text-grand-hotel text-bold">
          Quasagram
        </q-toolbar-title>

        <q-btn 
         class = "large-screen-only"
          to =  "/"
          icon="eva-home-outline" size="18px"  flat round dense/>

        
      </q-toolbar>
    </q-header>

    <q-footer
      class="bg-white small-screen-only"
      bordered
    >
       
          <q-tabs 
          class=text-grey-10
          active-color="primary"
          indicator-color="transparent"
          >
        <q-route-tab
          to="/"
          icon="eva-home-outline"
         
          
        />
       <q-route-tab
          to="/camera"
          icon="eva-camera-outline"
         
          
        />
        
      </q-tabs>
        
    </q-footer>

    <q-page-container class="bg-grey-1">
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>




export default {
  name: 'MainLayout',
 
  data () {
    return {
     
    }
  }
}
</script>

<style lang="sass" >

  .q-toolbar
     @media (min-width: $breakpoint-sm-min)
      height: 77px

  .q-footer
    .q-tab__icon
      font-size:  30px

  .q-toolbar__title
    @media (max-width: $breakpoint-xs-max)
      text-align: center
    font-size: 30px
  
  

</style>