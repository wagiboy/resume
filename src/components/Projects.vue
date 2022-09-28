<template>
  <div>
    <v-row>
      <v-col>
        <p class="display-2 primary--text font-weight-medium text-center pt-5">
          Projects
        </p>

      </v-col>
    </v-row>

    <!-- open source resumee -->
    <v-card class="mx-auto ma-0" max-width="1000">
      
      <v-card-text>
        <v-row>
          <v-col cols="12" sm="7">
            <p class="text-h5">
              Open Sourced This Résumé
            </p>
            Open Sourced and available on my GitHub page

            A VUEjs-based and powered-by-Vuetify (material UI kit) résumé template which you're seeing right now.
          </v-col>
          <v-col cols="12" sm="5" class="pa-0">
            <v-img
              src="@/assets/resumee.png"
             
             
            ></v-img>
          </v-col>
        </v-row>          
      </v-card-text>
    </v-card>


  </div>
</template>

<script>
export default {
 data: () => ({
   
 })        
}
</script>
