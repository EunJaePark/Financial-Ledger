<template>
  <!-- 로그인 페이지 -->
  <div class="regist-form login-form">
    <div class="regist-form-cont">
      <h3>SIGN IN</h3>
      <form class="form" action="">
        <!-- 아이디 -->
        <div>
          <label for="username">ID</label>
          <input id="username" type="text" />
        </div>
        <!-- 비밀번호 -->
        <div>
          <label for="password">PASSWORD</label>
          <input id="password" type="text" @click.prevent="" />
        </div>
        <!-- 회원정보 까먹었을때 찾는 버튼 -->
        <p><a href="" class="font-jua">Forgat password?</a></p>
        <button class="add-btn font-jua">add</button>
      </form>
      <button class="reset-btn" @click.prevent="resetEvent()">
        되돌아가기
      </button>
    </div>

    <a href="" class="mask login" @click.prevent="clickEvent()">
      <i class="icon"></i>
      <strong class="font-jua">SIGN IN</strong>
    </a>
  </div>
</template>
<script>
export default {
  data() {
    return {
      status: true,
      username: '',
      password: '',
    };
  },
  methods: {
    clickEvent() {
      const htmlElm = document.querySelector('html');
      const loginCont = htmlElm.querySelector(
        '.login-form > .regist-form-cont',
      );
      const signupCont = htmlElm.querySelector(
        '.signup-form > .regist-form-cont',
      );
      const signupForm = htmlElm.querySelector('.signup-form');
      const loginForm = htmlElm.querySelector('.login-form');
      const loginMask = htmlElm.querySelector('.login-form > .mask');
      const signupMask = htmlElm.querySelector('.signup-form > .mask');

      this.status = !this.status;
      if (!this.status) {
        loginForm.style.width = `${50 + 30}%`;
        signupForm.style.width = `${50 - 30}%`;

        signupForm.classList.add('active');

        loginCont.style.display = 'block';
        loginMask.style.display = 'none';
        signupCont.style.display = 'none';
        signupMask.style.display = 'block';
      }
    },
    resetEvent() {
      const loginCont = document.querySelector(
        '.login-form > .regist-form-cont',
      );
      const signupCont = document.querySelector(
        '.signup-form > .regist-form-cont',
      );
      const signupForm = document.querySelector('.signup-form');
      const loginForm = document.querySelector('.login-form');
      const loginMask = document.querySelector('.login-form > .mask');
      const signupMask = document.querySelector('.signup-form > .mask');

      this.status = true;

      if (this.status) {
        signupForm.style.width = `${50}%`;
        loginForm.style.width = `${50}%`;

        loginForm.classList.remove('active');
        signupForm.classList.remove('active');

        signupMask.style.display = 'block';
        signupCont.style.display = 'none';

        loginCont.style.display = 'none';
        loginMask.style.display = 'block';
      }
    },
    // overEvent() {
    //   const signupForm = document.querySelector('.signup-form');
    //   const loginForm = document.querySelector('.login-form');

    //   loginForm.style.width = `${50 + 20}%`;
    //   loginForm.style.transition = `all 0.6s ease`;

    //   signupForm.style.width = `${50 - 20}%`;
    //   loginForm.style.transition = `all 0.6s ease`;
    // },
    // outEvent() {
    //   const signupForm = document.querySelector('.signup-form');
    //   const loginForm = document.querySelector('.login-form');
    //   if (this.status) {
    //     loginForm.style.width = `${50}%`;
    //     loginForm.style.transition = `all 0.6s ease`;

    //     signupForm.style.width = `${50}%`;
    //     loginForm.style.transition = `all 0.6s ease`;
    //   }
    // },
  },
};
</script>
