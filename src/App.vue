<template>
  <div id="app">
    <app-header></app-header>
    <main>
      <h1>
        <span class="size">успей приобрести</span> <br>
			  путевки от <span class="price-color">70 000 &#8381;
			  </span>
      </h1>
      <timber></timber>
    </main>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import Timber from './components/Timber.vue'

export default {
  name: 'app',
  components: {
    AppHeader,
    Timber
  }
}
</script>

<style>
htm {
  height: 100vh;
}
  body {
    background: url(./assets/bg.jpg);
    overflow-x: hidden;
    background-size: cover;
    background-repeat: no-repeat;
    text-transform: uppercase;
    font-family: "Segoe UI Black";
    height: 100vh;
  }
  h1 {
    text-align: center;
    color: #184a6f;
    font-size: 58px;
    font-family: "Segoe UI Black";
  }
  .size {
      font-size: 50px;
  }
  .price-color {
      color: #ff1a14;
  }

</style>
