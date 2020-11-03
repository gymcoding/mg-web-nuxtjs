<template>
  <v-app class="grey">
    <v-app-bar height="56" color="primary" dark fixed app flat>
      <v-btn icon dark @click="$router.back()">
        <v-icon >mdi-arrow-left</v-icon>
      </v-btn>
      <v-toolbar-title v-text="'모두의발전기'" />
    </v-app-bar>
    <v-main>
      <v-container fill-height fluid>
        <v-row align="center" justify="center">
          <v-col cols="12" sm="8">
            <v-item-group>
              <v-container>
                <v-row>
                  <v-col
                    v-for="(item, index) in items"
                    :key="index"
                    cols="12"
                  >
                    <v-card :to="`/requests/write?requestType=${item.value}`" ripple>{{ item.text }}</v-card>
                    <!-- <v-item v-slot="{ active, toggle }">
                      <v-card
                        :color="active ? 'primary' : ''"
                        @click="toggle"
                      >
                      <v-layout>
                        <v-flex></v-flex>
                      </v-layout>
                        {{ item.text }}
                      </v-card>
                    </v-item> -->
                  </v-col>
                </v-row>
              </v-container>
            </v-item-group>
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
