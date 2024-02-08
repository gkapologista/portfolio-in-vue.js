<template>
  <div>
    <div v-for="(item, index) in progressData" :key="index">
      <div class="progressTitle">{{ item.title }}</div>
      <div class="progressBarContainer">
        <div class="progressBar" :style="{ width: item.progress + '%', backgroundColor: item.color }"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    progressData: {
      type: Array,
      required: true
    }
  }
}
</script>

<style lang="scss">

  .progressTitle {
    font-family: 'Montserrat', sans-serif, monospace;
    font-size: 16px;
    text-align: left;
    color: #FBFADA;
    margin-bottom: 8px;
  }

  .progressBarContainer {
    width: 40%;
    height: 16px;
    background-color: #FBFADA;
    border-radius: 10px;
    overflow: hidden;
    margin-bottom: 10px;
  }

  .progressBar {
    height: 100%;
    background-color: #4caf50;
    transition: width 0.3s ease;
  }

</style>
