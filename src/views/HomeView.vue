<template>
  <v-app :style="{ background: $vuetify.theme.themes.dark.background }">
    <Navbar />
    <v-container fluid>
      <v-row>
        <v-col cols="6">
          <v-img src="../assets/images/me.jpg" contain></v-img>
        </v-col>
        <v-col cols="6">
          <h5 class="red--text text--darken-4 top">Hello I'm Ethan</h5>
          <h1 class="white--text front">Front-End Developer</h1>
          <p class="grey--text">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. <br />
            Adipisci explicabo, cupiditate necessitatibus iure hic omnis est ab
            <br />
            At nihil et temporibus ratione!
          </p>
          <v-btn tile color="#A7121D" dark> about me </v-btn>
        </v-col>
      </v-row>
    </v-container>
  </v-app>

  <!-- <HelloWorld /> -->
</template>

<script>
import { defineComponent } from "vue";

// Components
// import HelloWorld from "../components/HelloWorld.vue";
import Navbar from "@/components/Navbar.vue";

export default defineComponent({
  name: "HomeView",

  components: {
    // HelloWorld,
    Navbar,
  },
});
</script>
<style lang="scss" scoped>
.top {
  margin-top: 180px;
  color: white;
}
.front {
  color: white;
  width: 10em;
  overflow: hidden;
  white-space: nowrap;
  animation: typing 6s steps(19), caret 1s steps(1) infinite;
}

@keyframes typing {
  from {
    width: 0;
  }
}
@keyframes caret {
  50% {
    border-right-color: transparent;
  }
}
</style>
