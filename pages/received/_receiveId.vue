<template>
  <v-app class="grey">
    <v-app-bar height="56" color="primary" dark fixed app flat>
      <v-btn icon dark @click="$router.back()">
        <v-icon >mdi-arrow-left</v-icon>
      </v-btn>
      <v-toolbar-title v-text="'받은 견적목록'" />
    </v-app-bar>
    <v-main>
      <v-container>
        <v-card>
          <v-card-text>
            <div>업체명</div>
            <div>인천 연수구</div>
            <div class="font-weight-bold">40,000원</div>
            <v-divider class="my-5"></v-divider>
            <div>동해물과 백두산이 ~~~</div>
            <v-row>
              <v-col><v-btn depressed block large color="primary" to="/received/complete">거래하기</v-btn></v-col>
              <v-col><v-btn depressed block large color="dark" to="/chats/2">문의하기</v-btn></v-col>
            </v-row>
            
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
