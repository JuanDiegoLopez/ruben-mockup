<template>
  <v-app>
    <v-toolbar  dark color="primary">
      <v-toolbar-title>Infosequence</v-toolbar-title>
    </v-toolbar>
    <v-container>
      <p class="title">Digita los parámetros de selección que usan espacio como separador, separados con comas.</p>
      <v-text-field label="Parametros de selección que usan espacio" required></v-text-field>
      
      <br>
      <p class="title">Digita los parámetros de selección que usan el signo = como separador, separados por comas.</p>
      <v-text-field label="Parametros de selección que usan =" required></v-text-field>
      <br><br>
      
      <v-layout row wrap>
        <v-flex xs6 class="px-2">
          <v-btn color="warning" block >Cargar datos</v-btn>
        </v-flex>
        <v-flex xs6 class="px-2">
          <v-btn color="primary" block>Generar tabla</v-btn>
        </v-flex>
      </v-layout>
    </v-container>
  </v-app>
</template>

<script>
  export default {
    data () {
      return {
        clipped: false,
        drawer: true,
        fixed: false,
        items: [
          { icon: 'bubble_chart', title: 'Inspire' }
        ],
        miniVariant: false,
        right: true,
        rightDrawer: false,
        title: 'Vuetify.js'
      }
    }
  }
</script>
