<template>
  <v-app>
    <v-main>
      <ChallengeList :itemsList="avaliableChallenges"/>
    </v-main>
  </v-app>
</template>

<script setup lang="ts">
import {ref} from "vue"
import ChallengeList from "./components/ChallengeList.vue"

const avaliableChallenges = [
  'Name Generator',
]

</script>
