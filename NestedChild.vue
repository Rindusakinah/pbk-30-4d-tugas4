<template>
    <div>
      <h3>Nested Component</h3>
      <button @click="selectItem('Item 1')">click 1</button>
      <button @click="selectItem('Item 2')">click 2</button>
    </div>
  </template>
  
  <script>
  export default {
    methods: {
      selectItem(item) {
        this.$emit('item-clicked', item);
      },
    },
  };
  </script>
  
  <style scoped>
  /* Tambahkan styling sesuai kebutuhan */
  </style>
  