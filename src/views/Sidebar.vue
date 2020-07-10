<template>
  <div class="sidebar-wrap">
    <SideGnbForm></SideGnbForm>
  </div>
</template>

<script>
import SideGnbForm from '@/components/common/SideGnbForm.vue';
export default {
  components: {
    SideGnbForm,
  },
};
</script>

<style>
.sidebar-wrap {
  width: 20%;
  display: inline-block;
  /* background-color: bisque; */
  height: 500px;
}
</style>
