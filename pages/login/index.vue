<template>
  <v-app class="grey">
    <v-app-bar height="56" color="primary" dark fixed app flat>
      <v-btn icon dark @click="$router.back()">
        <v-icon >mdi-arrow-left</v-icon>
      </v-btn>
      <v-toolbar-title v-text="'회원가입'" />
    </v-app-bar>
    <v-main class="white">
      <v-container>
        <v-text-field
          outlined
          placeholder="휴대전화 번호 또는 이메일을 입력해주세요."
        >
        </v-text-field>
        <v-text-field
          outlined
          placeholder="비밀번호를 입력해주세요."
        >
        </v-text-field>
        <v-btn class="mt-4" large block color="primary" depressed>로그인</v-btn>
        <nuxt-link to="/login/findPassword">비밀번호를 잊으셨나요?</nuxt-link>
        <v-btn class="mt-4" large block color="primary" depressed to="/signup">회원가입 하기</v-btn>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  data: () => ({
    chip: 0
  })
}
</script>

<style>

</style>
