<template>
  <div class="timber">
    <div class="timber__group">
      <crab></crab>
      <button class="timber__group-btn">в лето</button>
    </div>
	</div>
</template>

<script>
import Crab from './Crab.vue'

export default {
  components: {
    Crab
  }
}
</script>

<style>
  .timber {
    text-align: center;
    position: relative;
    max-width: 575px;
    height: 204px;
    margin: 0 auto;
    background: url(../assets/timber.png);
    margin-top: 100px;
  }
  .timber__group {
      position: absolute;
      top: -35%;
      left: 20%;
  }
</style>

