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
            <div>요청구분</div>
            <div>제목입니다.</div>
          </v-card-text>
        </v-card>
        <v-divider class="my-6"></v-divider>
        <v-card
          v-for="(item, index) in 10"
          class="mt-4"
          :key="index"
          to="/received/2"
        >
          <v-card-text>
            <div>업체명입니다.</div>
            <div>25,000원</div>
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
