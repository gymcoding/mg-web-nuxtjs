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
        <div class="font-weight-bold text-6">
          회원탈퇴를 하기전 아래 안내 사항을 확인해주세요.
        </div>
        <div class="grey--text text-subtitle-2">
          <div class="mt-2">1. 회원 탈퇴 시, 현재 로그인된 아이디는 즉시 탈퇴 처리가 요청됩니다.</div>
          <div class="mt-2">2. 회원 탈퇴 시 작성했던 리뷰는 삭제되지 않습니다.</div>
          <div class="mt-2">3. 회원 탈퇴 시 회원정보 및 서비스 이용 기록은 복구되지 않습니다.</div>
          <div class="mt-2">4. 소비자보호에 관한 법률 제6조에 의거, 계약 또는 청약철회등에 관한 기록은 5년, 대금결제 및 재화등의 공급에 관한 기록은 5년, 소비자의 불만 또는 분쟁처리에 관한 기록은 3년 동안 보관됩니다. 동 개인정보는 법률에 의한 보유 목적 외에 다른 목적으로는 이용되지 않습니다.</div>
          <div class="mt-2">5. 탈퇴 후 10일 동안 재가입할 수 없습니다.</div>
        </div>
        <v-divider class="my-5"></v-divider>
        <div class="font-weight-bold text-6">
          탈퇴하려는 이유가 무엇인가요?
        </div>
        <v-select
          :items="items"
          label="Outlined style"
          outlined
        ></v-select>
        <v-textarea
          outlined
          placeholder="소중한 의견 부탁드립니다."
        ></v-textarea>
        <div class="font-weight-bold text-6">
          정말 계정을 삭제하시겠어요?
        </div>
        <v-row dense>
          <v-col>
            <v-btn large depressed block outlined>더 사용해볼래요</v-btn>
          </v-col>
          <v-col>
            <v-btn large depressed block dark color="red">네, 삭제할게요</v-btn>
          </v-col>
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  data: () => ({
    chip: 0,
    switch1: false
  })
}
</script>

<style>

</style>
