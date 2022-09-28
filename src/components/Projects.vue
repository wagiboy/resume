<template>
  <div>
    <v-row>
      <v-col>
        <p class="display-2 primary--text font-weight-medium text-center py-5">
          Projects
        </p>
      </v-col>
    </v-row>

    <!-- open source resumee -->
    <v-card class="bluegrey--text mx-auto ma-0" max-width="900"> 
      <v-card-text>
        <v-row>
          <v-col cols="12" sm="7">
            <p class="text-h5 bluegrey--text font-weight-medium">
              Open Sourced This Résumé
            </p>
            <p class="bluegrey--text text-body-1">
              Open Sourced and available on my 
              <v-btn 
                text
                class="bluegrey--text text-capitalize font-weight-normal text-body-1 px-0"
                href="https://github.com/wagiboy/resume"
                target="_blank"
              > 
                GitHub page
                <v-icon class="bluegrey--text align-self-center">mdi-open-in-new</v-icon>
              </v-btn>
            </p>
            <p class="bluegrey--text text-body-1">

              A VUEjs-based and powered-by-Vuetify (material UI kit) résumé template which you're seeing right now.
            </p>
          </v-col>
          <v-col cols="12" sm="5" class="pa-0">
            <v-img src="@/assets/resumee.png"></v-img>
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
