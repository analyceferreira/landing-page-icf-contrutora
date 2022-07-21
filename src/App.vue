<script setup>
  import { ref } from 'vue'
  import header from './components/header.vue'


</script>


<template>
  <header/>
  <div class="videoWrapper">
    <iframe src="https://grupoicf.com.br/widgets/experts" allowfullscreen="" class=""></iframe>
  </div>
</template>


<style scoped>

.videoWrapper {
    position: relative;
    padding-bottom: 56.25%;
    padding-top: 25px;
    height: 0;
    overflow: hidden;
}
</style>
