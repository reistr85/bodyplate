<template>
  <v-card flat tile style="z-index: 999">
    <v-toolbar :dark="modeDark.value">
      <v-app-bar-nav-icon></v-app-bar-nav-icon>
      <v-toolbar-title>Title</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-switch v-model="modeDark.value" :label="modeDark.label" class="mt-6 mr-5"></v-switch>
      <v-btn icon><v-icon>mdi-dots-vertical</v-icon></v-btn>
    </v-toolbar>
  </v-card>
</template>

<script>
export default {
  name: 'NavBar',
  props: {
    modeDark: {
      type: Object,
      default: () => {},
      require: true
    }
  },
  data() {
    return {
    }
  }
}
</script>

<style>

</style>