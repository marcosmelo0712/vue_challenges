<template>
  <v-container>
    <v-navigation-drawer permanent>
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="text-h6">Challenges list</v-list-item-title>
          <!-- <v-list-item-subtitle>subtext</v-list-item-subtitle> -->
        </v-list-item-content>
      </v-list-item>

      <v-divider></v-divider>

      <v-list dense nav>
        <v-list-item v-for="item in props.itemsList" :key="item" link>
          <v-list-item-content>
            <v-list-item-title>{{ item }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
  </v-container>
  <!-- Component of the selected Item will be here: -->
  <v-container>
    
    <NameGenerator v-if="selectedItem == "/>
  </v-container>
</template>

<script setup lang="ts">
import logo from "../assets/logo.svg";
import { ref } from "vue"
import NameGenerator from "@/components/NameGenerator.vue"


// const mensagem = ref("teste mensagem")
// const props = defineProps(['itemList'])

const props = defineProps<{
  itemsList: Array<string>,
}>()

var selectedItem = 'Name Generator'

// console.log(props)

// const items = itemsList
const right = null

// __________-------TO DO: Change this component to be the home view, and make all the operations inside it, instead of using props

</script>
