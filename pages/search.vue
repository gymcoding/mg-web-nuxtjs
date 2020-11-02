<template>
  <v-app class="grey">
    <v-app-bar
      class="border-custom"
      color="primary"
      fixed
      flat
      app
      extended
      height="56"
      extension-height="100"
      :style="{
        borderColor: `${$vuetify.theme.themes.light.border} !important`
      }"
      >
      <v-toolbar-title class="white--text font-weight-bold" @click="$router.push('/')" v-text="'모두의발전기'" />
      <template v-slot:extension>
        <v-layout column white>
          <v-flex>
            <v-card class="d-inline-block mb-3" flat tile ripple @click="$refs.addressStageModal.open()">
              <v-layout align-center>
                <v-flex class="text-h6 font-weight-bold">인천 연수구</v-flex>
                <v-flex><v-icon color="black" :size="26">mdi-chevron-down</v-icon></v-flex>
              </v-layout>
            </v-card>
          </v-flex>
          <v-flex>
            <v-chip
              label
              outlined
              ripple
            >
              임대, 수리, 구매
            </v-chip>
          </v-flex>
        </v-layout>
      </template>
    </v-app-bar>
    <v-main>
      <v-divider class="mt-4 grey lighten-3"></v-divider>
      <v-container fluid white pa-0>
        <v-card class="pa-3" color="white" flat tile>
          <v-layout>
            <v-flex text-body-2>총 232개의 업체가 있어요</v-flex>
            <v-flex text-body-2 shrink>최신순</v-flex>
          </v-layout>
        </v-card>
        <v-divider></v-divider>
        <v-row dense no-gutters>
          <v-col
            v-for="(item, index) in 20"
            :key="index"
            cols="12"
            >
            <v-divider  v-if="index !== 0"></v-divider>
            <company-card>
            </company-card>
          </v-col>
        </v-row>
      </v-container>
      <address-stage-modal ref="addressStageModal"></address-stage-modal>
      <bottom-navigation></bottom-navigation>
    </v-main>
  </v-app>
</template>

<script>
import BottomNavigation from '@/components/BottomNavigation'
import CompanyCard from '@/components/CompanyCard'
import AddressStageModal from '@/components/AddressStageModal'
export default {
  components: {
    BottomNavigation,
    CompanyCard,
    AddressStageModal
  },
  created () {
  }
}
</script>

<style lang="scss">
.v-toolbar__extension {
  background: white;
}
.border-custom {
  border-color: var(--v-primary-base)
}
</style>
