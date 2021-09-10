<script setup>
defineProps({
  result: Boolean
})
</script>

<template>
  <div class="card">
    <div class="result" :class="result ? 'result-victory' : 'result-defeat'">
      <h1>{{ result ? 'Victory' : 'Defeat' }}</h1>
    </div>
    <div class="match-info">
      <div class="champion">
        <img alt="ChampionIcon" src="../assets/Champie_Vayne_profileicon.png" class="icon" />
      </div>
      <div class="match-details">
        <div class="score">
          <h2>10/10/6</h2>
        </div>
        <div class="queue">
          <h3>Solo</h3>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.icon {
  height: 100px;
  width: 100px;
}

.match-info {
  display: flex;
  flex-flow: row;
  height: 80%;
}

.match-details {
  display: flex;
  width: 50%;
  flex-flow: column;
}

.champion {
  padding-left: 5%;
  align-self: center;
}

.champion img {
  border-radius: 50%;
}

.score {
  justify-self: center;
  align-self: center;
}

.queue {
  justify-self: center;
  align-self: center;
}

.card {
    flex: 0 0 auto;
    display: flex;
    flex-flow: column;
    width: 15%;
    margin-left: 1.5%;
    margin-right: 1.5%;
    border-radius: 5%;
    background-color: gainsboro;
}

.result {
    justify-self: center;
    height: 20%;
    width: 100%;
}

.result h1 {
  margin: 0;
}

.result-victory {
    color: green;
}

.result-defeat {
    color: red;
}
</style>
