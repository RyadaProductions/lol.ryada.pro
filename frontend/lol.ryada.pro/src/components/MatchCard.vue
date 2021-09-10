<script setup>
defineProps({
  result: Boolean
})
</script>

<template>
  <div class="card" :class="result ? 'result-victory' : 'result-defeat'" >

    <div class="result">
      <h1>{{ result ? 'Victory' : 'Defeat' }}</h1>
    </div>
  </div>
</template>

<style scoped>

.card {
    flex: 0 0 auto;
    display: flex;
    width: 15%;
    margin-left: 1.5%;
    margin-right: 1.5%;
}

.result {
    justify-self: center;
}

.result-victory {
    background-color: green;
}

.result-defeat {
    background-color: red;
}
</style>
