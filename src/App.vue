<script setup>
import { RouterView } from "vue-router";
import TheNavBar from "@/components/TheNavBar.vue";
import TheFooter from "@/components/TheFooter.vue";
</script>

<template>
  <TheNavBar />
  <RouterView />
  <TheFooter />
</template>

<style>
body {
  background-color: white;
}
</style>
