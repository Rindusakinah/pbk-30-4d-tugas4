<template>
  <div id="app">
    <parent-component />
  </div>
</template>

<script>
import ParentComponent from './components/Parent.vue';

export default {
  name: 'App',
  components: {
    ParentComponent,
  },
};
</script>

<style>
/* Tambahkan styling sesuai kebutuhan */
</style>
