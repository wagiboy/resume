<template>
  <div>
    <!-- intro -->
    <v-row>
      <v-col>
        <v-img
          alt="Dirk Wagner at his desk"					
          src="@/assets/dirk-wagner.jpg"				
          contain
        />
          
        <p class="display-2 primary--text font-weight-medium text-center pt-5">
          Dirk Wagner
        </p>

        <p class="text-center bluegrey--text">
          An Experienced Web3 Dapp Developer
        </p>
      </v-col>
    </v-row>

    <!----- Info ----->
    <p class="bluegrey--text text--lighten-2 text-h5 mt-10 mb-3 mx-6">Info</p>

    <v-row class="ml-5" v-for="(info, i) in infoList" :key="i">
      <v-col cols="2" class="text-center">
        <v-icon class="bluegrey--text align-self-center">mdi-{{ info.icon }}</v-icon>
      </v-col>
      <v-col cols="10" :class="`bluegrey--text pt-${info.pt}`">
        <v-btn 
          v-if="info.link"
          text
          :class="`bluegrey--text ${info.class} px-0 font-weight-normal text-body-1`"
          :href="info.link"
          target="_blank"
        > 
          {{ info.name }}
        </v-btn>
        <v-span v-else>{{ info.name }}</v-span>
      </v-col>
    </v-row>

    <!----- Skills ----->
    <p class="bluegrey--text text--lighten-2 text-h5 mt-15 mb-3 mx-6">Skills</p>
    
    <v-row v-for="(skill, i) in skillList" :key="i" class="mx-7">
      <v-col>
        <p class="bluegrey--text ma-0">{{ skill.name }}</p>
        <v-progress-linear color="primary" height="3" :value="skill.percentage" />
      </v-col>
    </v-row>                                      
  </div>
</template>

<script>
export default {
 data: () => ({
    infoList: [{
      icon: 'email-outline',
      name: 'dirk@tutorz.com',
      link: '',
      class: '',
      pt: '3'
    },{
      icon: 'phone',
      name: '+49 175 6276 6272',
      link: '',
      class: '',
      pt: '3'
    },{
      icon: 'map-marker',
      name: 'Burgstädt, Germany',      
      link: 'https://www.burgstaedt.de/',
      class: 'text-capitalize',
      pt: '2'
    },{
      icon: 'github',
      name: 'github.com/wagiboy',      
      link: 'https://github.com/wagiboy',
      class: 'text-lowercase',
      pt: '2'      
    },{
      icon: 'instagram',
      name: 'instagram.com/wagiboy',      
      link: 'https://www.instagram.com/wagiboy/',
      class: 'text-lowercase',
      pt: '2' 
    }],

    skillList: [{
      icon: '',
      name: 'Cryptography',
      percentage: '60'
    },{
      icon: '',
      name: 'Web 3 development',
      percentage: '50'
    },{
      icon: '',
      name: 'Web 2 development',
      percentage: '90'
    },{            
      icon: '',
      name: 'VUEjs framework',
      percentage: '95'
    },{            
      icon: '',
      name: 'LAMP stack',
      percentage: '90'
    },{            
      icon: '',
      name: 'Python',
      percentage: '40'
    },{            
      icon: '',
      name: 'Perl',
      percentage: '70'
    },{            
      icon: '',
      name: 'Object-oriented design and development',
      percentage: '90'
    },{            
      icon: '',
      name: 'Parallel and distributed computing',
      percentage: '60'
    },{            
      icon: '',
      name: 'Protocol development',
      percentage: '40'
    },{            
      icon: '',
      name: 'Test-driven development',
      percentage: '80'
    },{            
      icon: '',
      name: 'Web application security',
      percentage: '40'
    },{            
      icon: '',
      name: 'Relational databases',
      percentage: '80'
    }]
 })        
}
</script>
