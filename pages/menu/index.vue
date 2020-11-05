<template>
  <v-app class="grey">
    <v-app-bar height="56" color="primary" dark fixed app flat>
      <v-toolbar-title v-text="'모두의발전기'" />
    </v-app-bar>
    <v-main>
      <v-container>
        <v-card ripple to="/signup">
          <v-card-text>
            <div class="font-weight-bold text-h6">로그인 / 회원가입</div>
          </v-card-text>
        </v-card>
        <v-card ripple to="/account">
          <v-card-text>
            <v-layout row align-center>
              <v-flex shrink>
                <v-icon color="primary" :size="30">mdi-home-circle-outline</v-icon>
              </v-flex>
              <v-flex><div class="font-weight-bold text-h6">닉네임님 안녕하세요</div> </v-flex>
              <v-flex shrink>
                <v-icon>mdi-chevron-right</v-icon>
              </v-flex>
            </v-layout>
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
</style>
