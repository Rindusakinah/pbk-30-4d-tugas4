<template>
    <div>
      <slot name="header"></slot>
      <h2>Child Component</h2>
      <nested-child @item-clicked="itemClicked" />
    </div>
  </template>
  
  <script>
  import NestedChild from './NestedChild.vue';
  
  export default {
    components: {
      NestedChild,
    },
    methods: {
      itemClicked(item) {
        this.$emit('item-selected', item);
      },
    },
  };
  </script>
  
  <style scoped>
  /* Tambahkan styling sesuai kebutuhan */
  </style>
  