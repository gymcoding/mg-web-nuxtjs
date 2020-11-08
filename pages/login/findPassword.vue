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
        <v-layout align-start>
          <v-flex>
            <v-text-field
              outlined
              placeholder="인증번호를 입력해주세요."
            >
            </v-text-field>
          </v-flex>
          <v-flex shrink pt-2 pl-2>
            <v-btn large depressed disabled>확인</v-btn>
          </v-flex>
        </v-layout>
        <v-text-field
          outlined
          placeholder="새로운 비밀번호"
        >
        </v-text-field>
        <v-btn class="mt-4" large block color="primary" depressed>비밀번호 재설정</v-btn>
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
