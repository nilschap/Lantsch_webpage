<template>
  <v-app>
    <v-main>
      <login/>
    </v-main>
  </v-app>
</template>

<script>
import login from './components/login.vue'

export default {
  name: 'App',
 
  components: {
    login,
  },

  data: () => ({
    //
  }),
}
</script>
