<template>
  <v-container>
    <v-row>
      <v-col cols="12" md="4" class="pa-0 mr-15">
        <SideBar />
      </v-col>
      <v-col cols="12" md="7" class="pl-15 py-15">
        <Body />
      </v-col>
    </v-row>
    <v-row>
      <v-col class="px-0 py-8">
        <Projects />
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import SideBar  from '@/components/SideBar.vue'
import Body     from '@/components/Body.vue'
import Projects from '@/components/Projects.vue'

export default {
  components: { SideBar, Body, Projects },  
  data: () => ({ 
  })
}
</script>

<style>
.underline {
  border-bottom:3px solid #aaa
}
</style>

