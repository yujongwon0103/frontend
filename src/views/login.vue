<template>
  <main class="form-signin w-100 m-auto">
    <form>
      <img class="mb-4" src="@/assets/logo.png" alt="" width="72" height="57">
      <div class="form-floating mt-3">
        <input type="email" class="form-control" id="inputEmail" placeholder="name@example.com">
        <label for="floatingInput">이메일</label>
      </div>
      <div class="form-floating">
        <input type="password" class="form-control" id="inputPassword" placeholder="Password">
        <label for="floatingPassword">비밀번호</label>
      </div>
      <div class="form-check text-start my-3">
        <input class="form-check-input" type="checkbox" value="" id="chkSaveEmail">
        <label class="form-check-label" for="checkDefault">이메일 저장</label>
      </div>
      <button class="btn btn-primary w-100 py-2" type="submit">로그인</button>
      <ul class="nav col-12 col-md-auto mt-3 mb-2 justify-content-center mb-md-0">
        <li><a href="javascript:void(0);" class="nav-link px-2 link-secondary" id="linkSignUp">회원가입</a></li>
        <li><a href="javascript:void(0);" class="nav-link px-2 link-secondary" id="linkFindAccount">계정 찾기</a></li>
        <li><a href="javascript:void(0);" class="nav-link px-2 link-secondary" id="linkFindPassword">비밀번호 찾기</a></li>
      </ul>
      <button class="btn" type="button" id="btnNaverLogin" @click="onBtnNaverLoginClick">
        <img src="@/assets/naver_login.png">
      </button>
      <button class="btn" type="button" id="btnKakaoLogin">
        <img src="@/assets/kakao_login.png">
      </button>
      <button class="btn" type="button" id="btnAppleLogin">
        <img src="@/assets/apple_login.png">
      </button>
      <p class="mt-5 mb-3 text-body-secondary">© Y.J.W.</p>
    </form>
  </main>
</template>
<script lang="ts" setup>
  import { ref, onMounted } from 'vue'

  function onBtnNaverLoginClick() {
    let param : Object = {
      response_type: "code",
      client_id: "Um9MhjncgTDxOgo2OnH0",
      redirect_uri: "http://localhost:8080/login",
      state: ""
    }
  }

  onMounted(() => {

  })
</script>