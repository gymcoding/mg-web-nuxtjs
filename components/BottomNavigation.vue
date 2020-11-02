<template>
  <v-bottom-navigation
    color="primary"
    grow
    app
  >
    <v-btn height="56" to="/">
      <span>홈</span>
      <v-icon>mdi-home-outline</v-icon>
    </v-btn>

    <v-btn height="56" to="/search">
      <span>업체찾기</span>
      <v-icon>mdi-magnify</v-icon>
    </v-btn>

    <v-btn height="56" to="/requests">
      <span>이용내역</span>
      <v-icon>mdi-file-outline</v-icon>
    </v-btn>
  </v-bottom-navigation>
</template>

<script>
export default {
  data: () => ({
    value: 1
  })
}
</script>

<style>

</style>