<template>
  <div class="app-header">
    <img src="../assets/logo.png" alt="">
      <div class="plane">
        <div class="plane__img">
            <img src="../assets/plane.png" alt="">
        </div>
      </div>
  </div>
</template>

<style>
  .app-header {
    text-align: center;
  }
  .logo > img{
      display: inline-block;
      max-width: 100%;
      text-align: center;
  }
  .plane {
      position: absolute;
      left: -7%;
      top: 3%;
      width: 114%;
      font-size: 4rem;
  }
  .plane__img {
      position: relative;
      width: 1em;
      left: 0;
      font-family: Arial;
      animation: plane 20s infinite;
      animation-timing-function: linear;
  }
  @keyframes plane {
    49% {
        left: calc(100% - 1em);
        transform: scaleX(1); 
    }
    50% {
        transform: scaleX(-1);
    }
    100% {
        transform: scaleX(-1);
    }
  }
</style>

