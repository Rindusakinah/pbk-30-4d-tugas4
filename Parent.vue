<template>
    <div>
      <h1>Component induk </h1>
      <child-component @item-selected="handleItemSelected">
        <template v-slot:header>
          <h2></h2>
        </template>
      </child-component>
      <p>Selected Item: {{ selectedItem }}</p>
    </div>
  </template>
  
  <script>
  import ChildComponent from './Child.vue';
  
  export default {
    components: {
      ChildComponent,
    },
    data() {
      return {
        selectedItem: null,
      };
    },
    methods: {
      handleItemSelected(item) {
        this.selectedItem = item;
      },
    },
  };
  </script>
  
  <style scoped>
  /* Tambahkan styling sesuai kebutuhan */
  </style>
  