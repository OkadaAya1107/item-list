<template>
<ul>
  <li v-for="item in items" :key="item.id">{{ item.id }} - {{ item.name }}</li>
</ul>
</template>

<!-- Option API -->
<!-- <script> 
export default {
  //プロップスでリストデータを親から受け取る
  props: ['items'],
};

</script> -->

<!-- Composition API NEW -->
<script setup>
import { defineProps } from 'vue';

const props = defineProps(['items']);
</script>

<style>
</style>