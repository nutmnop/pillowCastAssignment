<template>
  <div id="app">
    <b-navbar variant="faded" id="navbar">
      <b-navbar-brand to="/" tag="h1" class="mb-0">
         <img src="../src/assets/p.png" width="10%" >
         Pillow Cast
      </b-navbar-brand>
      <b-navbar-nav class="ml-auto">
        <b-nav-item to="/">Help</b-nav-item>
        <b-nav-item to="/">Cast Out</b-nav-item>
        <b-nav-item to="/">Upload Cast</b-nav-item>
      </b-navbar-nav>
    </b-navbar> 
     
    <router-view/>
   
  </div>
</template>

<script>


export default {
  components: {
    
  }
}
</script>


<style lang="scss">
#app {
  font-family: 'Bree Serif', serif;

  color: white;
  background-color: #132233;
}
#navbar {
 a{
   color: whitesmoke;
 } 
}
</style>
