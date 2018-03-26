<template>
  <div class="crab">
    <div class="crab__wrapper">
      <div class="crab__img">
        <div class="crab__img-body"></div>
        <div class="crab__img-eye"></div>
        <div class="crab__img-eye2"></div>
        <div class="crab__img-leye"></div>
        <div class="crab__img-reye"></div>
        <div class="crab__img-lfoot"></div>
        <div class="crab__img-rfoot"></div>
        <div class="crab__img-lhand"></div>
        <div class="crab__img-rhand"></div>
        <div class="crab__img-shell"></div>
      </div>
    </div>
  </div>
</template>

<style>
  .crab {
    left: 20%;
    width: 220px;
    font-size: 4rem; 
  } 
  .crab__wrapper {
    width: 220px;
    position: relative;
    width: 10px;
    left: 0;
    font-family: Arial;
    animation: 4s linear 0s infinite alternate crab;
  }
  .crab__img {
      position: relative;
      width: 180px;
      height: 150px;
  }
  .crab__img-body {
      position: absolute;
      width: 79px; height: 45px;
      background: url('../assets/crab.png') -128px -10px;
      left: 30%;
      top: 55%;
      z-index: 1;
  }
  .crab__img-eye {
      position: absolute;
      width: 12px; height: 8px;
      background: url('../assets/crab.png') -199px -146px;
      top: 70%;
      left: 38%;
      z-index: 3;
  }
  .crab__img-eye2 {
      position: absolute;
      width: 12px; height: 8px;
      background: url('../assets/crab.png') -199px -146px;
      top: 70%;
      left: 59%;
      z-index: 3;
  }
  .crab__img-leye {
      position: absolute;
      width: 20px; height: 17px;
      background: url('../assets/crab.png') -227px -95px;
      top: 70%;
      left: 38%;
      z-index: 2;
  }
  .crab__img-reye {
      position: absolute;
      width: 20px; height: 17px;
      background: url('../assets/crab.png') -159px -146px;
      top: 70%;
      left: 55%;
      z-index: 2;
  }
  .crab__img-lfoot {
      position: absolute;
      width: 50px; height: 65px;
      background: url('../assets/crab.png') -227px -10px;
      top: 54%;
      left: 9%;
      z-index: 1;
      animation: rotateLeft .2s infinite linear;
  }
  .crab__img-rfoot {
      position: absolute;
      width: 50px; height: 65px;
      background: url('../assets/crab.png') -10px -146px;
      top: 54%;
      left: 66%;
      z-index: 1;
      animation: rotateRight .2s infinite linear;
  }
  .crab__img-lhand {
      position: absolute;
      width: 59px; height: 43px;
      background: url('../assets/crab.png') -128px -75px;
      left: 17%;
      top: 73%;
      z-index: 3;
  }
  .crab__img-rhand {
      position: absolute;
      width: 59px; height: 43px;
      background: url('../assets/crab.png') -80px -146px;
      left: 54%;
      top: 73%;
      z-index: 3;
  }
  .crab__img-shell {
      position: absolute;
      width: 98px; height: 116px;
      background: url('../assets/crab.png') -10px -10px;
      left: 25%;
  }
  @keyframes crab { 
    from {
        margin-left: 0% 
    } 
    to { 
        margin-left: calc(100% - 10px); 
    } 
  }
  @keyframes rotateRight {
    from {
        transform: rotate(31deg);
        transform-origin: bottom left;
    }
    to {
        transform: rotate(0deg);
        transform-origin: bottom left;
    }
  }
  @keyframes rotateLeft {
      from {
          transform: rotate(0deg);
          transform-origin: bottom right;
      }
      to {
          transform: rotate(-31deg);
          transform-origin: bottom right;
      }
  }
</style>
