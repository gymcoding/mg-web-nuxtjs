<template>
  <v-app class="grey">
    <v-app-bar height="56" color="primary" dark fixed app flat>
      <v-btn icon dark @click="$router.back()">
        <v-icon >mdi-arrow-left</v-icon>
      </v-btn>
      <v-toolbar-title v-text="'견적서 선택'" />
    </v-app-bar>
    <v-main>
      <v-row align="center" justify="center">
        <v-col>
          <v-btn>발전기 임대</v-btn>
        </v-col>
      </v-row>
    </v-main>
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
