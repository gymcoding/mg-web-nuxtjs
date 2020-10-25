<template>
   <v-card
      @click="$router.push('/companies/23')"
    >
      <div class="d-flex flex-no-wrap">
        <v-avatar
          class="ma-3"
          size="125"
          tile
        >
          <v-img :src="item.src"></v-img>
        </v-avatar>
        <div>
          <v-card-text>
            <div class="title font-weight-bold">삼성발전기</div>
            <div>경기도 하남시</div>
            <div>#구매 #수리</div>
            <v-btn>문의하기</v-btn>
          </v-card-text>
        </div>
      </div>
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
