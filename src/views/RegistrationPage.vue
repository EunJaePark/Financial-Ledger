<template>
  <!-- 회원등록 페이지 -->
  <div class="registration-page-wrap no-header">
    <LoginForm></LoginForm>
    <SignupForm></SignupForm>
  </div>
</template>

<script>
import LoginForm from '@/components/registration/LoginForm';
import SignupForm from '@/components/registration/SignupForm';

export default {
  components: {
    LoginForm,
    SignupForm,
  },
};
</script>

<style></style>
