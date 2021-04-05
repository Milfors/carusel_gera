<template>
    <div>
        <v-card width="700" class="mx-auto" elevation="30">
            <v-list-item>
                <v-list-item-content>
                    <v-list-item-label>
                    <v-img
                    src="https://www.lahza.ma/aptoaloo/2019/04/La-stratégie-marketing-de-Xiaomi-en-2018-1.png"
                    height="100px"
                    width="650px"
                    >
                    </v-img>
                    </v-list-item-label>

                    <vue-list-title>
                        <p>Интернет магазин Mi</p>
                        <h6>
                        <h2>Redmi 9T</h2>
                        </h6>
                    </vue-list-title>

                <v-img
                justify-end
                src="https://droid-market.ru/image/catalog/opisanie/phone/mi_9t_pro_1.jpg"
                height="700px"
                width="600px"
                 >
                 </v-img>
                </v-list-item-content>
                <v-list-item-action>
                </v-list-item-action>
            </v-list-item>

            <v-card-actions>
                 <v-btn
                        class="mx-2"
                        icon
                        dark
                        
                        small
                        color="red"
                >
                    
                 </v-btn>
                 <v-btn
                        class="mx-9"
                        
                        dark
                        
                        color="orange"
                        @click="Show = !Show">
                     >
                        <v-icon orange>
                         mdi-comment-account-outline
                         
                         </v-icon>
                         
                         
                     </v-btn>
                     <h2>Характеристики</h2>
                    <v-spacer></v-spacer>
                    

            </v-card-actions>
            
            <div>
                <Carusel v-show="Show"/>
            </div>
        </v-card>
    </div>
    
</template>

<script>
import Carusel from './Carusel'
export default {
    name: "Slide",
    components:{
        Carusel
    },
    data: function(){
        return{
            Show: false
        }
    }

}

</script>
<style>
.label-img {
    margin: 50px;
    padding: 0;
    position: relative;
    width:64px;
    height:64px;
    background: #ec5a5a;
    border: 1px solid rgb(74, 226, 61);
    border-radius:3px;
}
</style>