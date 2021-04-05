<template>
  <v-carousel
      :continuous="false"
      :cycle="cycle"
      :show-arrows="true"
      
      hide-delimiter-background
      
      delimiter-icon="mdi-minus"
      height="280"
    >
      <v-carousel-item
        v-for="(Comment, i) in Comments"
        :key="i"
      >
      <v-sheet
      color= white
      height = "20%"
      >
          <Comment :Com="Comment"/>
          </v-sheet>
      </v-carousel-item>
    </v-carousel>
</template>

<script>
import Comment from './Comment.vue'
export default {
    name: 'Carusel',
    components:{
      Comment
    },
    data: function(){
        return{
            model: 0,
          Comments: [
            {
                UserName: 'Дисплей - ', Massage: '6.53 2340x1080 (19.5:9) 395 ppi IPS', Image: "https://static.onlinetrade.ru/img/items/s/smartfon_xiaomi_mi_9t_pro_6_128gb_glacier_blue_1158786_1.jpg"
            },
            {
                UserName: 'Аппаратная часть -  ', Massage: 'Android 10.0 Snapdragon 662', Image: "https://img2.freepng.ru/20190430/vhz/kisspng-central-processing-unit-portable-network-graphics-helplessacemyrielectrics-icon-processor-is-a-goodi-5cc7cac5e5c1b5.7322786715565974459411.jpg"
            },
            {
                UserName: 'Результаты тестов - ', Massage: 'AnTuTu Benchmark 175411 баллов', Image: "https://avatars.mds.yandex.net/get-zen_doc/1866022/pub_5cb057a84f78f300b344c270_5cb057dd6f22e100b29c3470/scale_1200"
            }
          ]
        }
    }
}
</script>

<style>
</style>