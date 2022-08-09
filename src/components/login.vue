<script>
export default {
  data() {
    return {
      awesome: true
    }
  },
  methods: {
    toggle() {
      this.awesome = !this.awesome
    }
  }
}
</script>

<template>
<div fill-height fluid align="center">
    <v-container fill-height fluid align="center">
        <v-row>
            <v-col></v-col>
            <v-col>
                <h1 v-if="awesome">Vue is awesome!</h1>
                <h1 v-else>Oh no 😢</h1>
                <h1 style="color: black; font-family: 'EB Garamond', serif;">Lantsch lenz</h1>
                <v-text-field label="Registration code" width=15%></v-text-field>
                <v-btn @click.native="toggle" elevation="2" >Login</v-btn>
                <button @click="toggle">toggle</button>
            </v-col>
            <v-col></v-col>
        </v-row>
    </v-container>
</div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=EB+Garamond&display=swap');
.content {
  margin: 0;
  position: absolute;
  top: 40%;
  left:50%;
  transform: translate(-50%, -50%);
}
.bg {
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    background: url('https://arosalenzerheide.swiss/1-content-hauptseiten/02_lenzerheide/region/wissenwertes/orte-plaene/lantsch-lenz/image-thumb__21448974__header-sujet/sommer.in-lantsch-lenz.jpg') no-repeat center center;
    background-size: cover;
    transform: scale(1.1);
  }
</style>

