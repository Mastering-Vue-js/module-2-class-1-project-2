<script setup>
import { ref } from "vue";
const x = ref(0)
const y = ref(0)
const result = ref(0)
</script>
<template>
  <div class="calculator">
    <input type="number" name="x" v-model="x" />
    <input type="button" @click="result = x+y" name="add" value="+" />
    <input type="button" @click="result = x-y" name="minus" value="-" />
    <input type="button" @click="result = x*y" name="multiply" value="*" />
    <input type="button" @click="result = x/y" name="divided" value="/" />
    <input type="number" name="y" v-model="y" />
    <input type="button" name="" value="=" />
    <input type="number" name="result" v-model="result" />
  </div>
</template>
<style>
</style>