<template>
  <v-app class="grey">
    <v-app-bar height="56" color="primary" dark fixed app flat>
      <v-btn icon dark @click="$router.back()">
        <v-icon >mdi-arrow-left</v-icon>
      </v-btn>
      <v-toolbar-title v-text="'계정관리'" />
    </v-app-bar>
    <v-main class="white">
      <v-container>
        <div>
          <div class="font-weight-bold">현재 비밀번호</div>
          <v-text-field
            outlined
            placeholder="8자리 이상 영문자,숫자,특수문자 포함"
            hide-details
          >
          </v-text-field>
        </div>
        <div class="mt-5">
          <div class="font-weight-bold">비밀번호</div>
          <v-text-field
            outlined
            placeholder="8자리 이상 영문자,숫자,특수문자 포함"
            hide-details
          >
          </v-text-field>
          <v-text-field
            outlined
            placeholder="비밀번호 확인"
          >
          </v-text-field>
        </div>
      </v-container>
    </v-main>
    <v-footer color="grey lighten-3" app>
      <v-btn depressed large block color="primary">확인</v-btn>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data: () => ({
  }),
  methods: {
    doLogout () {
    }
  }
}
</script>

<style>

</style>
