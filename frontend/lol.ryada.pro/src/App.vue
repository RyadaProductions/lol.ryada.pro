<script setup>
import SummonerDetails from './components/SummonerDetails.vue';
import MatchCarousel from './components/MatchCarousel.vue';
</script>

<template>
  <SummonerDetails summonerName="Ryada" />
  <MatchCarousel />
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
