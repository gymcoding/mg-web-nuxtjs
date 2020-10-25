<template>
  <v-row dense>
    <v-col
      v-for="(item, index) in 20"
      :key="index"
      cols="12"
      sm="6"
      >
      <company-card>
      </company-card>
    </v-col>
  </v-row>
</template>

<script>
import CompanyCard from '@/components/CompanyCard'
export default {
  components: {
    CompanyCard
  }
}
</script>

<style>

</style>
