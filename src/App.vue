<template>
  <div id="app">
    <Sidebar></Sidebar>
    <StatusHeader></StatusHeader>
    <router-view class="router-area"></router-view>
  </div>
</template>

<script>
import Sidebar from '@/views/Sidebar.vue';
import StatusHeader from '@/views/StatusHeader.vue';
export default {
  components: {
    Sidebar,
    StatusHeader,
  },
};
</script>

<style>
@import url('./assets/css/reset.css');
@import url('./assets/css/common.css');
@import url('./assets/css/main-page.css');
@import url('./assets/css/statistics-page.css');
</style>
