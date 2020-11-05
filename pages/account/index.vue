<template>
  <v-app class="grey">
    <v-app-bar height="56" color="primary" dark fixed app flat>
      <v-btn icon dark @click="$router.back()">
        <v-icon >mdi-arrow-left</v-icon>
      </v-btn>
      <v-toolbar-title v-text="'휴대전화 번호'" />
    </v-app-bar>
    <v-main class="white">
      <v-container>
        <v-card ripple>
          <v-card-text>
            <v-layout align-center>
              <v-flex font-weight-bold>이메일</v-flex>
              <v-flex shrink>sohryong@gmail.com</v-flex>
            </v-layout>
          </v-card-text>
        </v-card>
        <v-card ripple to="/account/phoneNumber">
          <v-card-text>
            <v-layout align-center>
              <v-flex font-weight-bold>휴대전화 번호</v-flex>
              <v-flex shrink>010-****-0107</v-flex>
              <v-flex shrink>
                <v-icon>mdi-chevron-right</v-icon>
              </v-flex>
            </v-layout>
          </v-card-text>
        </v-card>
        <v-card to="/account/password">
          <v-card-text>
            <v-layout align-center>
              <v-flex font-weight-bold>비밀번호 재설정</v-flex>
              <v-flex shrink>
                <v-icon>mdi-chevron-right</v-icon>
              </v-flex>
            </v-layout>
          </v-card-text>
        </v-card>
        <v-card>
          <v-card-text class="py-0">
            <v-layout align-center>
              <v-flex font-weight-bold>마케팅 정보 수신 동의</v-flex>
              <v-flex shrink>
                <v-switch
                ></v-switch>
              </v-flex>
            </v-layout>
          </v-card-text>
        </v-card>
        <v-btn block large depressed outlined @click="doLogout">로그아웃</v-btn>
        <div>탈퇴를 원하시면 <nuxt-link to="/account/withdraw">여기</nuxt-link>를 눌러주세요.</div>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  data: () => ({
    chip: 0,
    switch1: false
  }),
  methods: {
    doLogout () {
      this.$confirm('로그아웃 하시겠습니까?').then(result => {
        if (result) {
          this.$router.push('/')
        }
      })
    }
  }
}
</script>

<style>

</style>
