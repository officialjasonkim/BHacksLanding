<template>
  <nav>
    <v-app-bar app>
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>
      <v-toolbar-title>
        <img
          class="mr-3"
          :src="require('@/assets/BostonHacksMark.png')"
          height="30"
        />
        BostonHacks
      </v-toolbar-title>
    </v-app-bar>

    <v-navigation-drawer app v-model="drawer">
      <v-list nav dense>
        <v-list-item-group v-model="group" active-class=" text--accent-4">
          <v-toolbar-items>
            <v-btn text @click="home()">Home</v-btn>
            <v-btn
              v-if="this.getRoutePath && this.getRoutePath == '/'"
              text
              href="#schedule"
              >Schedule</v-btn
            >
            <v-btn
              v-if="this.getRoutePath && this.getRoutePath == '/'"
              text
              href="#tracks"
              >Tracks and Workshops</v-btn
            >
            <v-btn
              v-if="this.getRoutePath && this.getRoutePath == '/'"
              text
              href="#FAQ"
              >FAQ</v-btn
            >
            <v-btn text @click="application()">Application</v-btn>
            <v-btn icon>
              <v-icon v-if="user" @click="signOut()">mdi-export-variant</v-icon>
              <v-icon v-else @click="signIn()">mdi-arrow-right</v-icon>
            </v-btn>
          </v-toolbar-items>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </nav>
</template>

<script>
export default {
  name: "MobileBar",
  data() {
    return {
      drawer: false,
      group: 0
    };
  },
  computed: {
    user() {
      return this.$store.state.user;
    },
    getRoutePath() {
      return this.$route.path;
    }
  },
  methods: {
    async signOut() {
      await this.$store.dispatch("logOut");
      this.$router.push("/");
    },
    signIn() {
      this.$router.push("/login");
    },
    home() {
      this.$router.push("/");
    },
    application() {
      this.$router.push("/application");
    }
  }
};
</script>
