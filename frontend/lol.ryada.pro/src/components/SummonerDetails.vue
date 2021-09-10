<script setup>
defineProps({
  summonerName: String
})

const summonerLevel = 153;
const rank = 'Gold';
</script>

<template>
  <div class="header">
    <div class="profile">
      <img alt="ChampieVayne" src="../assets/Champie_Vayne_profileicon.png" class="icon rounded" />
      <div class="highlight-text">
        <h1>{{ summonerName }}</h1>
        Level: {{ summonerLevel }}
      </div>
    </div>
    <div class="profile">
      <img alt="GoldArmorSolo" src="../assets/gold_armor.png" class="icon" />
      <div class="highlight-text">
        <h1>{{ rank }}</h1>
        Solo
      </div>
    </div>
    <div class="profile">
      <img alt="GoldArmorFlex" src="../assets/gold_armor.png" class="icon" />
      <div class="highlight-text">
        <h1>{{ rank }}</h1>
        Flex
      </div>
    </div>
  </div>
</template>

<style scoped>
.rounded {
  border-radius: 50%;
}

.icon {
  width: 100px;
  height: 100px;
}

.header {
  display: flex;
  justify-content: space-evenly;
  width: 100%;
  padding-bottom: 25px;
  /* Remove background color after finishing design */
  background-color: bisque;
}

.profile {
  display: flex;
  flex-direction: row;

}

.highlight-text {
  padding-left: 10px;
  line-height: normal;
}

.highlight-text h1 {
  margin-bottom: 0px;
}
</style>
