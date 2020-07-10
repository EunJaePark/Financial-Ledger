<template>
  <!-- 사이드 GNB -->
  <div class="side-gnb-form">
    <!-- 로고 -->
    <div class="logo-cont">
      <h1><a href="">머니부</a></h1>
      <!-- <h1><a href="">moneyBoo</a></h1> -->
    </div>
    <!-- GNB Menu -->
    <div class="gnb-list-cont">
      <ul>
        <li
          v-for="(item, index) in gnblist"
          :class="[item.value, { active: item.active }]"
          :key="index"
          :disabled="item.value == 'transparent-bar'"
        >
          <a href="">
            <i class="gnb-icon" :class="item.value + '-icon'"></i
            >{{ item.ktext }}
          </a>
        </li>
      </ul>
    </div>
    <!-- calender -->
    <div class="calender-cont">
      <i></i>
      <span class="desc">날씨아이콘 / 날씨 정보</span>
      <strong class="date">10</strong>
      <span class="day">Friday</span>
      <span class="month">July, 2020</span>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      click: '',
      gnblist: [
        { text: 'Main', value: 'main', link: '/main', ktext: '메인' },
        {
          text: 'Daily',
          value: 'daily',
          link: '/daily',
          active: 'active',
          ktext: '데일리',
        },
        {
          text: 'Statistics',
          value: 'statistics',
          link: '/statistics',
          ktext: '통계',
        },
        {
          text: 'Settings',
          value: 'settings',
          link: '/setting',
          ktext: '관리',
        },
        {
          text: 'Transparent-bar',
          value: 'transparent-bar',
          link: '',
          ktext: '',
        },
        {
          text: 'Mypage',
          value: 'mypage',
          link: '/mypage',
          ktext: '마이페이지',
        },
        { text: 'Logout', value: 'logout', link: '', ktext: '로그아웃' },
      ],
    };
  },
  methods: {},
};
</script>

<style></style>
