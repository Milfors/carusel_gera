<template>
  <v-card width="520" class="mx-auto" elevation="1" >
      <v-list-item>
        <v-list-item-avatar>

            <v-img
            :src = "Com.Image"
        >
        </v-img>

        </v-list-item-avatar>
          <vue-list-title>
              
              {{Com.UserName}} {{Com.Massage}}
              
              <br /> 
              
          </vue-list-title>  
          <v-spacer></v-spacer>
      </v-list-item>
  </v-card>
</template>

<script>
export default {
    name: 'Comment',
    props: ['Com'],
}
</script>
<style>
</style>