<template>
  <!--회원가입 페이지  -->
  <div class="regist-form signup-form">
    <div class="regist-form-cont">
      <h3>SIGN UP</h3>
      <form action="">
        <!-- 아이디 -->
        <div>
          <label for="username">ID</label>
          <input id="username" type="text" />
        </div>
        <!-- 닉네임 -->
        <div>
          <label for="nickname">NICKNAME</label>
          <input id="nickname" type="text" />
        </div>
        <!-- 비밀번호 -->
        <div>
          <label for="password">PASSWORD</label>
          <input id="password" type="text" />
        </div>
        <button class="add-btn font-jua">add</button>
      </form>
      <button class="reset-btn" @click.prevent="resetEvent()">
        되돌아가기
      </button>
    </div>
    <a href="" class="mask signup" @click.prevent="clickEvent()">
      <i class="icon"></i>
      <strong class="font-jua">SIGN UP</strong>
    </a>
  </div>
</template>
<script>
export default {
  data() {
    return {
      status: true,
    };
  },
  methods: {
    clickEvent() {
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

      this.status = !this.status;
      if (!status) {
        signupForm.style.width = `${50 + 30}%`;
        loginForm.style.width = `${50 - 30}%`;

        loginForm.classList.add('active');

        signupMask.style.display = 'none';
        signupCont.style.display = 'block';

        loginCont.style.display = 'none';
        loginMask.style.display = 'block';
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

    //   signupForm.style.width = `${50 + 20}%`;
    //   loginForm.style.width = `${50 - 20}%`;
    // },
    // outEvent() {
    //   const signupForm = document.querySelector('.signup-form');
    //   const loginForm = document.querySelector('.login-form');

    //   if (this.status) {
    //     signupForm.style.width = `${50}%`;
    //     loginForm.style.width = `${50}%`;
    //   }
    // },
  },
};
</script>
