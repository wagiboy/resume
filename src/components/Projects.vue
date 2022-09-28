<template>
  <div>
    <v-row>
      <v-col>
        <p class="display-2 primary--text font-weight-medium text-center py-5">
          Recent Projects
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
              A VUEjs-based and powered-by-Vuetify (material UI kit) résumé template, which you're seeing right now.
            </p>
          </v-col>
          <v-col cols="12" sm="5" class="pa-0">
            <a href="http://tutorz.org">
              <v-img src="@/assets/resumee.png"></v-img>
            </a>
          </v-col>
        </v-row>          
      </v-card-text>
    </v-card>

    <!-- citadelia -->
    <v-card class="bluegrey--text mx-auto mt-7" max-width="900"> 
      <v-card-text>
        <v-row>
          <v-col cols="12" sm="7">
            <p class="text-h5 bluegrey--text font-weight-medium">
              Citadelia
            </p>
            <p class="bluegrey--text text-body-1">
              A blockchain-based public works funds management system. 
              <v-btn 
                text
                class="bluegrey--text text-lowercase font-weight-normal text-body-1 px-0"
                href="http://citadelia.city"
                target="_blank"
              > 
                http://citadelia.city
                <v-icon class="bluegrey--text align-self-center">mdi-open-in-new</v-icon>
              </v-btn>
            </p>
            <p class="bluegrey--text text-body-1">
              This project is a donation to the Free Cities Foundation&mdash;an organization, for which I serve as an ambassador.
            </p>
          </v-col>
          <v-col cols="12" sm="5" class="pa-0">
            <a href="http://citadelia.city">
              <v-img src="@/assets/citadelia.png" ></v-img>
            </a>      
          </v-col>
        </v-row>          
      </v-card-text>
    </v-card>

    <!-- ttz -->
    <v-card class="bluegrey--text mx-auto mt-7" max-width="900"> 
      <v-card-text>
        <v-row>
          <v-col cols="12" sm="7">
            <p class="text-h5 bluegrey--text font-weight-medium">
              TTZ Coin
            </p>
            <p class="bluegrey--text text-body-1">
              A cryptocurrency useful for purchasing tutoring and receiving rewards. 
              <v-btn 
                text
                class="bluegrey--text text-lowercase font-weight-normal text-body-1 px-0"
                href="http://tutorz.co"
                target="_blank"              
              > 
                http://tutorz.co
                <v-icon class="bluegrey--text align-self-center">mdi-open-in-new</v-icon>
              </v-btn>
            </p>          
          </v-col>
          <v-col cols="12" sm="5" class="pa-0  ">
            <a href="http://tutorz.co">
              <v-img 
                src="@/assets/ttz-coin.png" 
                width="200" 
                class="mx-auto mt-6"
              ></v-img>
            </a>      
          </v-col>
        </v-row>          
      </v-card-text>
    </v-card>    

    <!-- TutorZ -->
    <v-card class="bluegrey--text mx-auto mt-7" max-width="900"> 
      <v-card-text>
        <v-row>
          <v-col cols="12" sm="7">
            <p class="text-h5 bluegrey--text font-weight-medium">
              TutorZ
            </p>
            <p class="bluegrey--text text-body-1">
              Founded the tutor referral platform TutorZ.com. 
              Architected the site and business models. 
              Lead a team of 6 web developers, marketers, and customer service reps. 
              <v-btn 
                text
                class="bluegrey--text text-lowercase font-weight-normal text-body-1 px-0"
                href="http://www.tutorz.com"
                target="_blank"              
              > 
                https://tutorz.com
                <v-icon class="bluegrey--text align-self-center">mdi-open-in-new</v-icon>
              </v-btn>
            </p>          
          </v-col>
          <v-col cols="12" sm="5" class="pa-0">
            <a href="https://www.tutorz.com">
              <v-img 
                src="@/assets/tutorz.gif" 
                width="180" 
                class="mx-auto mt-12"
              ></v-img>
            </a>      
          </v-col>
        </v-row>          
      </v-card-text>
    </v-card>        

  </div>
</template>
