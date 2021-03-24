<template>
  <v-card width="600" class="mx-auto" elevation="10" >
      <v-list-item>
        <v-list-item-avatar>
            <v-img
            src = 'https://images.unsplash.com/photo-1586459023690-8bda067ff1bf?ixid=MXwxMjA3fDB8MHx0b3BpYy1mZWVkfDh8dG93SlpGc2twR2d8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=900&q=60'>
                
            </v-img>
        </v-list-item-avatar>
          <vue-list-title>
              {{Com.UserName}}  Комментит: {{Com.Massage}} 
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