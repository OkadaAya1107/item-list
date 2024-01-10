<template>
  <h1>Item List</h1>
<item-list :items="itemList"></item-list>
</template>

<!-- Option API -->
<!-- <script>
import ItemList from './components/ItemList.vue';
export default {
components: {
  ItemList,
 },
 data() {
  return {
    itemList: [
      {
       id: 1,
       name: 'Item 1',
    },
      {
       id: 2,
       name: 'Item 2',
    },
      {
       id: 3,
       name: 'Item 3',
    },
   ],
  };
 },
};
</script> -->

<!-- Composition API NEW -->
<script setup>
import ItemList from './components/ItemList.vue';

import { ref } from 'vue';

const itemList = ref([
{
       id: 1,
       name: 'Item 1',
    },
      {
       id: 2,
       name: 'Item 2',
    },
      {
       id: 3,
       name: 'Item 3',
    },
]);
</script>

<style>
</style>