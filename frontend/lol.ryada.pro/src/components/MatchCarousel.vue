<script setup>
import MatchCard from "./MatchCard.vue";
</script>

<template>
  <div class="carousel">
    <MatchCard v-bind:result="true" />
    <MatchCard v-bind:result="true" />
    <MatchCard v-bind:result="false" />
    <MatchCard v-bind:result="true" />
    <MatchCard v-bind:result="false" />
    <MatchCard v-bind:result="false" />
    <MatchCard v-bind:result="false" />
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
    background-color: darkgrey;
}
</style>
