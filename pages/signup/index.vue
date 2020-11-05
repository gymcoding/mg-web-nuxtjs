<template>
  <v-app class="grey">
    <v-app-bar height="56" color="primary" dark fixed app flat>
      <v-btn icon dark @click="$router.back()">
        <v-icon >mdi-arrow-left</v-icon>
      </v-btn>
      <v-toolbar-title v-text="'회원가입'" />
    </v-app-bar>
    <v-main>
      <v-container>
        <v-card>
          <v-card-text>
            <div class="font-weight-bold">휴대전화 번호</div>
            <div class="grey--text text-subtitle-2">거래예약이 확정된 업체에게만 연락처가 공개됩니다.</div>
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
            <div>
              <div class="font-weight-bold">이메일</div>
              <v-text-field
                outlined
                placeholder="helloworld@abc.kr"
              >
              </v-text-field>
            </div>
            <div>
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
            <v-checkbox
              label="이용약관 전체동의"
              hide-details
            ></v-checkbox>
            <v-checkbox
              label="[필수] 이용약관 및 개인정보 취급방침 동의"
              hide-details
            ></v-checkbox>
            <v-checkbox
              label="[필수] 만 14세 이상"
              hide-details
            ></v-checkbox>
            <v-checkbox
              label="이벤트 등 혜택/정보 수신"
              hide-details
            ></v-checkbox>
            <v-btn class="mt-4" large block color="primary" depressed>회원가입 완료</v-btn>
          </v-card-text>
        </v-card>
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
