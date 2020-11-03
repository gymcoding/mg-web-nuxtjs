<template>
  <v-app class="grey">
    <v-app-bar height="56" color="primary" dark fixed app flat>
      <v-toolbar-title v-text="'모두의발전기'" />
    </v-app-bar>
    <v-main>
      <v-container>
        <v-card
          v-for="(item, index) in 10"
          :key="index"
          :class="{ 'mt-4': index !== 0 }"
          to="/requests/request-01"
        >
          <v-card-text>
            <div>요청카테고리</div>
            <div class="font-weight-bold text-h6">제목입니다.</div>
          </v-card-text>
        </v-card>
      </v-container>
    </v-main>
    <bottom-navigation></bottom-navigation>
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
