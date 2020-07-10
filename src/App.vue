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
@import './assets/css/reset.css';
@import './assets/css/common.css';
@import './assets/css/daily-page.css';

/* @font-face {
  font-family: 'BBTreeGB';
  src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_nine_@1.1/BBTreeGB.woff')
    format('woff');
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: 'BBTreeGB';
  src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_nine_@1.1/BBTreeGB.woff')
    format('woff');
  font-weight: normal;
  font-style: normal;
} */

/* body {
  background-color: #fef2e4;
  font-family: 'Jua', sans-serif;
}
.app {
  width: 95%;
  position: relative;
  overflow: hidden;
  background-color: #348f6c;
  border-radius: 1em;
  height: 590px;
  margin: 0 auto;
  margin-top: 60px;
} */
/* .view-page { */
/* overflow-y: scroll; */
/* background-color: #ffffff; */
/* width: calc(80% - 90px); */
/* margin: 0.9em 0.9em 0.9em 0; */
/* margin: 10px 10px 10px 0; */
/* margin-top: 2.4em; */
/* height: 520px; */
/* height: 42.68em; */
/* border-radius: 1em; */
/* padding-top: 50px; */
/* } */
</style>
