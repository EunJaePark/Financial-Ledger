<template>
  <div class="app">
    <Sidebar></Sidebar>
    <StatusHeader></StatusHeader>
    <router-view></router-view>
  </div>
</template>

<script>
import Sidebar from "@/views/Sidebar.vue";
import StatusHeader from "@/views/StatusHeader.vue";
export default {
  components: {
    Sidebar,
    StatusHeader
  }
};
</script>

<style></style>
