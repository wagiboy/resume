<template>
  <v-app>
    <v-main>
      <router-view/>
    </v-main>
    <v-footer padless class="white">
      <v-col cols="12" class="text-center blue-grey--text caption">
        <v-icon small>mdi-xml</v-icon>
        {{ new Date().getFullYear() }} — Dirk Wagner
      </v-col>
    </v-footer>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>
