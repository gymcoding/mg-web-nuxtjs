<template>
  <v-app class="grey">
    <v-app-bar height="56" color="primary" dark fixed app flat>
      <v-btn icon dark @click="$router.back()">
        <v-icon >mdi-arrow-left</v-icon>
      </v-btn>
      <v-toolbar-title v-text="'대화하기'" />
    </v-app-bar>
    <v-main>
      <v-container>
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
