<template>
  <v-app class="grey">
    <v-app-bar height="56" color="primary" dark fixed app flat>
      <v-btn icon dark @click="$router.back()">
        <v-icon >mdi-arrow-left</v-icon>
      </v-btn>
      <v-toolbar-title v-text="'견적요청서'" />
    </v-app-bar>
    <v-main>
      <v-container fluid>
        <v-card class="pa-4">
          <v-select
            label="요청카테고리"
            :items="items"
            outlined
            placeholder="요청카테고리를 선택해주세요."
          ></v-select>
          <v-text-field
            label="요청 제목"
            placeholder="예) OOO 임대 견적 요청드립니다."
            outlined
          ></v-text-field>
          <v-textarea
            outlined
            label="요청 내용"
            placeholder="예) OOO 임대 견적 요청드립니다."
          ></v-textarea>
          <v-text-field
            label="연락처"
            outlined
            placeholder="'-' 없이 숫자만 입력해주세요."
          ></v-text-field>
          <v-btn large block color="primary" depressed to="/requests/complete">요청하기</v-btn>
        </v-card>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  components: {
  },
  data: () => ({
    items: [
      { text: '임대', value: '임대' },
      { text: '수리', value: '수리' },
      { text: '구매', value: '구매' },
    ]
  })
}
</script>
