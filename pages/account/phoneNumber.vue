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
        <div class="font-weight-bold">휴대전화 번호</div>
        <v-layout align-start>
          <v-flex>
            <v-text-field
              outlined
              placeholder="휴대전화 번호를 입력해주세요."
            >
            </v-text-field>
          </v-flex>
          <v-flex shrink pt-2 pl-2>
            <v-btn large depressed disabled>인증</v-btn>
          </v-flex>
        </v-layout>
        <v-text-field
          outlined
          placeholder="인증번호를 입력해주세요."
        >
        </v-text-field>
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
  })
}
</script>

<style>

</style>
