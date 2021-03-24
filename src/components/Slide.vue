<template>
    <div>
        <v-card width="600" class="mx-auto" elevation="15">
            <v-list-item>
                <v-list-item-content>
                <v-img
                justify-end
                src="https://images.unsplash.com/photo-1589878529966-c29b9e067b78?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=1653&q=80"
                >
                </v-img>
                <v-alert
                color="purple"
                elevation="10"
                icon="mdi-fire"
                >Внимание! Слишком милая картинка:)</v-alert>
                </v-list-item-content>
                <v-list-item-action>
                </v-list-item-action>
            </v-list-item>
            <v-card-actions>
                   <v-btn
                        class="mx-2"
                        fab
                        dark
                        cmall
                        color="teal"
                        @click="Show = !Show">
                     >
                        <v-icon dark>
                         mdi-comment-account-outline
                         </v-icon>
                     </v-btn>
                 <v-btn
                        class="mx-2"
                        fab
                        dark
                        small
                        color="pink"
                >
                    <v-icon dark>
                     mdi-heart
                     </v-icon>
                 </v-btn>
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
</style>