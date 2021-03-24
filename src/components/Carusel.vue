<template>
  <v-carousel
      :continuous="false"
      :cycle="cycle"
      :show-arrows="true"
      hide-delimiter-background
      delimiter-icon="mdi-minus"
      height="200"
    >
      <v-carousel-item
        v-for="(Comment, i) in Comments"
        :key="i"
      >
          <Comment :Com="Comment"/>
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
                UserName: 'Мартин', Massage: 'Какая прелесть!'
            },
            {
                UserName: 'Виктор', Massage: 'Нет слов)'
            },
            {
                UserName: 'Саймон', Massage: 'А кто может быть лучше?'
            }
          ]
        }
    }
}
</script>

<style>
</style>