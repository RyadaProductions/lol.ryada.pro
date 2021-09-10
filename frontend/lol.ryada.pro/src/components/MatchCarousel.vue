<script setup>
import MatchCard from "./MatchCard.vue";

const matches = [true, true, false, true, false, false, false, false, false, false]
</script>

<template>
  <div class="carousel">
    <MatchCard v-for="match in matches" :key="match" v-bind:result=match />
  </div>
</template>

<style scoped>
.carousel {
    display: flex;
    flex-wrap: nowrap;
    flex-flow: row;
    width: 100%;
    height: 200px;
    overflow: auto;
}
</style>
