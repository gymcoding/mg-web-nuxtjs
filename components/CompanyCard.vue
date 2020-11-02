<template>
  <v-card
    @click="$router.push('/companies/23')"
    flat
    tile
  >
    <v-layout pa-3>
      <v-flex shrink>
        <v-avatar
          size="110"
          tile
        >
          <v-img :src="item.src"></v-img>
        </v-avatar>
      </v-flex>
      <v-flex py-3 px-4>
        <div class="title font-weight-bold">삼성발전기</div>
        <div class="text-body-2 grey--text text--darken-1">경기도 하남시</div>
        <div>
          <v-chip
            v-for="(item, index) in ['구매', '수리', '임대']"
            class="ma-1 caption"
            color="grey lighten-4"
            :key="index"
            small
            >
            {{ item }}
          </v-chip>
        </div>

      </v-flex>
    </v-layout>
  </v-card>
</template>

<script>
export default {
  data: () => ({
    image: 'https://www.makervil.com/upload_files/company/5debd41a-e7c0-4c1f-8d79-1e9da5de1efe.png',
    item: {
      companyName: '삼성발전기',
      color: 'primary',
      src: 'https://phinf.pstatic.net/image.nmv/blog_2019_05_29_1429/47775570-81b4-11e9-bbd6-00000000464c_03.jpg?type=f238x238',
      title: 'Halcyon Days',
      artist: 'Ellie Goulding',
    }
  })
}
</script>

<style>

</style>
