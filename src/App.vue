<template>
  <v-app>
    <v-main>
      <ChallengeList :itemsList="avaliableChallenges"/>
      <h1>{{selectedChallenge}}</h1>
    </v-main>
  </v-app>
</template>

<script setup lang="ts">
import {ref} from "vue"
import ChallengeList from "./components/ChallengeList.vue"

var selectedChallenge = ref('____________')

const avaliableChallenges = [
  'Name Generator'
]

</script>
