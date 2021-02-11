<style scoped src="@/assets/topnav.css"></style>
<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view/> -->
    
      <div class="topnav">
          <div>
            <a class="navbar-brand logo-title" href="#">Logo</a>
          </div>
          <div class="ava">
              <img class="userava" src="@/assets/nav_img/ava.svg" alt="">
              <h5 class="username">Samsul Arifin</h5>
          </div>
          <div class="icon">
            <a href="#"><img src="@/assets/nav_img/Icon.svg" alt=""></a>
          </div>
      </div>
    
    <router-view/>
  </div>
</template>

