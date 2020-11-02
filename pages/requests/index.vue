<template>
  <v-app class="grey">
    <v-app-bar height="56" color="primary" dark fixed app flat>
      <v-toolbar-title v-text="'모두의발전기'" />
    </v-app-bar>
    <v-main>
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
