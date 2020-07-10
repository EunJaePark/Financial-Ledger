<template>
  <div class="setting-page-wrap">
    <SetAsset></SetAsset>
    <SetCategory></SetCategory>
  </div>
</template>

<script>
import SetAsset from '@/components/setting/SetAsset.vue';
import SetCategory from '@/components/setting/SetCategory.vue';

export default {
  components: {
    SetAsset,
    SetCategory,
  },
};
</script>

<style></style>
