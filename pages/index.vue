<template>
  <v-app class="grey">
    <v-app-bar height="56" color="primary" dark fixed app flat>
      <v-toolbar-title v-text="'모두의발전기'" />
    </v-app-bar>
    <v-main>
      <v-container px-5 text-center>
        <div class="py-8">
          <div class="grey--text mb-2">국내 최초 발전기 중개 플랫폼</div>
          <div class="font-weight-black" :style="{ lineHeight: '1.3em', fontSize: '2.5rem' }">
            터치 한번으로<br>
            견적을 가볍게
          </div>
        </div>
        <v-btn
          height="64px"
          min-width="240px"
          elevation="10"
          class="font-weight-bold"
          color="blue-grey darken-4"
          dark
          tile
          large
          :style="{ fontSize: '1.1rem' }"
          to="/requests/selection"
        >
          지금 견적 알아보기
        </v-btn>
      </v-container>
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
