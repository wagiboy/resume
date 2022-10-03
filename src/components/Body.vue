<template>
  <div>

    <!-- summary -->
    <p class="bluegrey--text underline">
      Web3 Developer Summary
    </p>

    <v-row v-for="(summary, i) in summaryList" :key="i" class="ml-3">
      <v-col cols="1" class="text-center px-0">
        <v-icon class="bluegrey--text align-self-center">mdi-{{ summary.icon }}</v-icon>
      </v-col>
      <v-col cols="11" class="bluegrey--text">
        {{ summary.text }}
      </v-col>
    </v-row>
    <div class="hidden-sm-and-down spacer"></div>

    <!-- education -->
    <p class="bluegrey--text underline mt-15">
      Education
    </p>

    <v-row v-for="(edu, i) in eduList" :key="i" class="ml-3">
      <v-col cols="1" class="text-center px-0">
        <v-icon class="bluegrey--text align-self-center">mdi-{{ edu.icon }}</v-icon>
      </v-col>
      <v-col cols="11" class="bluegrey--text">
        {{ edu.text }}
      </v-col>
    </v-row>
    <div class="hidden-sm-and-down spacer"></div>

    <!-- certificates -->
    <p class="bluegrey--text underline mt-15">
      Udemy Academy Certificates
    </p>

    <v-row v-for="(certificate, i) in certificateList" :key="i" class="mx-3">
      <v-col cols="1" class="text-center px-0">
        <v-icon class="bluegrey--text align-self-center">mdi-{{ certificate.icon }}</v-icon>
      </v-col>
      <v-col cols="10" class="bluegrey--text">
        {{ certificate.text }}
      </v-col>
      <v-col cols="1" class="bluegrey--text">
        <v-btn 
          text
          class="bluegrey--text"
          href="/certificates"
          target="_blank"
        > 
          <v-icon class="bluegrey--text align-self-center">mdi-open-in-new</v-icon>
        </v-btn>
      </v-col>
    </v-row>  
    <div class="hidden-sm-and-down spacer"></div>  

    <!-- spoken langauges -->
    <p class="bluegrey--text underline mt-15">
      Spoken Languages
    </p>

    <v-row class="mt-0 justify-center">
      <v-col cols="3" class="text-center">
        <v-progress-circular
          rotate="-90"
          size="80"
          width="2"
          value="96"
          color="primary"
          class="mx-auto"
        >
          <span class="bluegrey--text text-caption">English<br>20+ years</span>
        </v-progress-circular>
      </v-col>
      <v-col cols="3" class="text-center">
        <v-progress-circular
          rotate="-90"
          size="80"
          width="2"
          value="98"
          color="primary"
        >
          <span class="bluegrey--text text-caption">German<br>native</span>
        </v-progress-circular>
      </v-col>
      <v-col cols="3" class="text-center">
        <v-progress-circular
          rotate="-90"
          size="80"
          width="2"
          value="50"
          color="primary"
        >
          <span class="bluegrey--text text-caption">Russian<br>3 years</span>
        </v-progress-circular>
      </v-col>
    </v-row>
    <div class="hidden-sm-and-down spacer"></div> 

    <!-- programming langauges -->
    <p class="bluegrey--text underline mt-15">
      Programming Languages
    </p>

    <v-row class="mt-0 justify-center">
      <v-col cols="2" class="text-center">
        <v-progress-circular
          rotate="-90"
          size="80"
          width="3"
          value="95"
          color="primary"
          class="mx-auto"
        >
          <span class="bluegrey--text text-caption">PHP</span>
        </v-progress-circular>
      </v-col>
      <v-col cols="2" class="text-center">
        <v-progress-circular
          rotate="-90"
          size="80"
          width="3"
          value="85"
          color="primary"
        >
          <span class="bluegrey--text text-caption">C/C++</span>
        </v-progress-circular>
      </v-col>
      <v-col cols="2" class="text-center">
        <v-progress-circular
          rotate="-90"
          size="80"
          width="3"
          value="80"
          color="primary"
        >
          <span class="bluegrey--text text-caption">JavaScript</span>
        </v-progress-circular>
      </v-col>
      <v-col cols="2" class="text-center">
        <v-progress-circular
          rotate="-90"
          size="80"
          width="3"
          value="65"
          color="primary"
        >
          <span class="bluegrey--text text-caption">Solidity</span>
        </v-progress-circular>
      </v-col>      
    </v-row>
    <div class="hidden-sm-and-down spacer"></div>     

    <!-- tool/techonolgy chips -->
    <p class="bluegrey--text underline mt-15">
      Tools
    </p>

    <v-chip class="ma-2" color="primary" text-color="white" v-for="(chip, i) in chipList" :key="i">  
      <v-avatar v-if="chip.icon" left>
        <v-icon>mdi-{{ chip.icon }}</v-icon>
      </v-avatar>
      {{ chip.text }}
    </v-chip>    
  </div>
</template>

<script>
export default {
  data: () => ({
    summaryList: [{
      icon: 'currency-btc',
      text: 'Certified blockchain developer with hands-on experience of designing and implementing Solidity smart contracts using the Ethereum VM and Polygon blockchain',
    },{
      icon: 'ethereum',
      text: 'Ethereum node operator and staking portfolio manager',
    },{
      icon: 'web',
      text: 'Expert in LAMP-stack web development and web search',
    },{
      icon: 'server-network',
      text: 'Significant experience in object-oriented design and programming, algorithms and distributed computing',
    },{
      icon: 'account-supervisor',
      text: 'Strong relationship-building and leadership skills',
    },{
      icon: 'desktop-classic',
      text: 'M.S. in computer science',
    }],

    eduList: [{
      icon: 'school',
      text: 'M.S. in Computer Science, University of Erlangen-Nuremberg, Germany, 1996'
    },{
      icon: 'account-school',
      text: 'Research Assistant at the University of California at Santa Barbara, 1996',
    }],


    certificateList: [{
      icon: 'lock-open',
      text: 'Encryption and Cryptography, 4 hours of lectures, 2022'
    },{
      icon: 'link-lock',
      text: 'Building Blockchains, 15 hours of lectures, 2 projects, 2022',
    },{
      icon: 'ethereum',
      text: 'Ethereum and Solidity, 25 hours of lectures, 3 projects, 2022',      
    }],


    chipList: [{
      icon: 'microsoft-visual-studio-code',
      text: 'Visua Studio Code',
    },{
      icon: 'headset-dock',
      text: 'Remix',
    },{
      icon: 'github',
      text: 'GitHub',      
    },{
      icon: 'recycle',
      text: 'Alchemy',
    },{
      icon: 'cube',
      text: 'Ganache',      
    },{
      icon: 'dolphin',
      text: 'MariaDB',
    },{    
      icon: 'netflix',
      text: 'Nginx',
    },{            
      icon: 'feather',
      text: 'Apache',
    },{            
      icon: '',
      text: 'Photoshop',
    },{            
      icon: 'centos',
      text: 'CentOS',
    },{     
      icon: '',
      text: 'Vim',
    },{          
      icon: 'microsoft-windows',
      text: 'Windows NT-11',
    }]            
  })
};
</script>

<style>
.underline {
  border-bottom:3px solid #aaa
}
.spacer {
   height:2em
}
</style>

 