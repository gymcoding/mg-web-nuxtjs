<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="8">
      <v-card flat>
        <v-card flat>
          <v-layout>
            <v-flex shrink>
              <v-img :width="160" aspect-ratio="1" :src="'https://phinf.pstatic.net/image.nmv/blog_2019_05_29_1429/47775570-81b4-11e9-bbd6-00000000464c_03.jpg?type=f238x238'"></v-img>
            </v-flex>
            <v-flex pa-5>
              <div class="headline font-weight-bold">삼성발전기</div>
              <div class="mt-3 grey--text text--darken-1">대표 : 한소룡</div>
              <div class="grey--text text--darken-1">전화 : 032-858-6700</div>
              <div class="grey--text text--darken-1">주소 : 인천 연수구 송도동</div>
            </v-flex>
          </v-layout>
        </v-card>
      </v-card>
      <v-divider class="my-8"></v-divider>
      <v-card flat>
        <div class="headline font-weight-bold">업체소개</div>
        <div class="mt-3 grey--text text--darken-1">
          안녕하세요. 감사합니다. 저희는 삼성발전기 업체입니다.안녕하세요. 감사합니다. 저희는 삼성발전기 업체입니다.안녕하세요. 감사합니다. 저희는 삼성발전기 업체입니다.안녕하세요. 감사합니다. 저희는 삼성발전기 업체입니다.
        </div>
      </v-card>
      
      <v-divider class="my-8"></v-divider>
      <v-card flat>
        <div class="headline font-weight-bold">서비스 가능 항목</div>
        <div class="mt-3">
          <v-chip color="grey lighten-4" class="grey--text text--darken-1">
            발전기 임대
          </v-chip>
          <v-chip color="grey lighten-4" class="grey--text text--darken-1">
            발전기 수리
          </v-chip>
          <v-chip color="grey lighten-4" class="grey--text text--darken-1">
            발전기 판매
          </v-chip>
        </div>
      </v-card>
      <v-divider class="my-8"></v-divider>
      <v-card flat>
        <div class="headline font-weight-bold">서비스 가능 지역</div>
        <div class="mt-3 grey--text text--darken-1">
          인천 전체 / 서울 관악구 / 서울 노원구 / 부산 전체
        </div>
      </v-card>
      <v-divider class="my-8"></v-divider>
      <v-card flat>
        <div class="headline font-weight-bold">서비스 상세(사례) 보기</div>
        <v-chip-group
          v-model="chip"
          active-class="primary--text font-weight-bold"
          column
        >
          <v-chip
            v-for="(item, index) in ['발전기 임대', '발전기 수리', '발전기 판매']"
            :key="index"
            outlined
          >
            {{ item }}
          </v-chip>
        </v-chip-group>
        <div class="mt-3">
          <v-row dense>
            <v-col cols="4" sm="3">
              <v-img src="https://phinf.pstatic.net/image.nmv/blog_2019_05_29_1429/47775570-81b4-11e9-bbd6-00000000464c_03.jpg?type=f238x238"></v-img>
            </v-col>
            <v-col cols="4" sm="3">
              <v-img src="https://phinf.pstatic.net/image.nmv/blog_2019_05_08_1620/d6b65723-715a-11e9-913f-28b4484d5a96_03.jpg?type=f238x238"></v-img>
            </v-col>
            <v-col cols="4" sm="3">
              <v-img src="https://postfiles.pstatic.net/MjAxOTAzMTRfNDEg/MDAxNTUyNTQ0OTYzNTMy.C3UjGSwnKLs9Y2e-eqU_xPcBSI1XxPgwkncyFFnODrgg.fWkanyzifsvCfI84PxtLPkXaQyi60CoTZHr_bBym9o8g.JPEG.youngam61/KakaoTalk_20190103_095936421.jpg?type=f238"></v-img>
            </v-col>
            <v-col cols="4" sm="3">
              <v-img src="https://phinf.pstatic.net/image.nmv/blog_2019_05_07_1944/8c01465f-7057-11e9-bbd6-00000000464c_03.jpg?type=f238x238"></v-img>
            </v-col>
            <v-col cols="4" sm="3">
              <v-img src="https://postfiles.pstatic.net/MjAxOTAzMDdfMTI0/MDAxNTUxOTIzOTU3MTIy.-KgyPTMqB6jU3yZS6cf2aZ4sj2ngWILI6iMk2LkqN1Ig.aUcLo8hRhTEUydCv2nO6aua_LWa87fe6G54wsPM2BHwg.JPEG.youngam61/images5LMI7T2K.jpg?type=f238"></v-img>
            </v-col>
            <v-col cols="4" sm="3">
              <v-img src="https://postfiles.pstatic.net/MjAxOTAzMDZfMTc0/MDAxNTUxODUyNzk4NDg3.fHnJs6MY3MJoy6w6MPyFm_JSYgyOSuXvwmiZcL9n5f8g.AxFa0aCc4fcdEKlMjjkxwzBm0xqzsi40TKxCZJ4Lzzkg.JPEG.youngam61/KakaoTalk_Moim_55Ji7TL5hAQZ2gr5P6sn0dAjLDItzk.jpg?type=f238"></v-img>
            </v-col>
          </v-row>
        </div>
      </v-card>
      <v-divider class="my-8"></v-divider>
      <v-card flat>
        <div class="headline font-weight-bold">기본정보</div>
        <div class="mt-3">
          <v-layout>
            <v-flex shrink>설립일자 : </v-flex>
            <v-flex>1500</v-flex>
          </v-layout>
          <v-layout>
            <v-flex shrink>업종 : </v-flex>
            <v-flex>1500</v-flex>
          </v-layout>
          <v-layout>
            <v-flex shrink>업태 : </v-flex>
            <v-flex>1500</v-flex>
          </v-layout>
        </div>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
  data: () => ({
    chip: 0
  })
}
</script>

<style>

</style>
