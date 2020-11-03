<template>
  <v-app class="grey">
    <v-app-bar height="56" color="primary" dark fixed app flat>
      <v-toolbar-title v-text="'모두의발전기'" />
      <v-spacer></v-spacer>
      <v-btn icon dark @click="$router.push('/')">
        <v-icon>mdi-close</v-icon>
      </v-btn>
    </v-app-bar>
    <v-main>
      <v-container fill-height fluid>
        <v-row align="center" justify="center">
          <v-col>
            <v-card class="pa-4">
              <div class="text-center mb-5">
                거래가 완료되었습니다.
              </div>
              <v-btn depressed block large color="primary" to="/requests">확인</v-btn>
            </v-card>
          </v-col>
        </v-row>
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
      { text: '발전기 임대', value: 'generator_lease' },
      { text: '발전기 수리', value: 'generator_repair' },
      { text: '발전기 구매', value: 'generator_purchase' },
    ]
  })
}
</script>
