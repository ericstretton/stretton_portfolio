<template>
    <v-footer
    color="primary lighten-1"
    padless
    
  >
    <v-row
      justify="center"
      no-gutters
    >
    
      
      <v-btn text class="darkslategrey--text">
        LinkedIn
      </v-btn>

      <v-divider vertical></v-divider>

      <v-btn text class="darkslategrey--text">
        GitHub
      </v-btn>

      <v-divider vertical></v-divider>

      <v-btn text class="darkslategrey--text">
        Attributes
      </v-btn>

      <v-divider vertical></v-divider>
    

      
      <v-col
        class="primary lighten-2 py-4 text-center darkslategrey--text"
        cols="12"
      >
      
        <weak class="darkslategrey--text">©</weak> 
        {{  new Date().getFullYear()  }} — 
        <strong class="darkslategrey--text">Web Development by Eric Stretton</strong>
      </v-col>
    </v-row>
  </v-footer>
</template>

<script>
    export default {
        name: "PageFooter",
        data: () => ({
      links: [
        'LinkedIn',
        'GitHub',
        'Attributes'
      ],
    }),
    }
</script>

<style lang="scss" scoped>

</style>