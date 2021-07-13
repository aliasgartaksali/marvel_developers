<template>
  <v-app>
    <v-app-bar app color="black" dark>
      <v-app-bar-nav-icon @click.stop="sidebarMenu = !sidebarMenu">
      </v-app-bar-nav-icon>
      <v-toolbar-title>
        <v-row>
          <v-col>
            <v-img
              transition="scale-transition"
              alt="Marvel Logo"
              src="./assets/logo-white.svg"
            />
          </v-col>
          <v-col><h3 style="font-color: white">| Developers</h3></v-col>
        </v-row>
      </v-toolbar-title>

      <v-spacer></v-spacer>
      <v-btn rounded color="white" dark class="black--text">
        Sign up free
      </v-btn>
    </v-app-bar>
    <v-navigation-drawer
      v-model="sidebarMenu"
      app
      floating
      :permanent="sidebarMenu"
      color="black"
    >
      <v-list style="color: white">
        <v-list-item>
          <v-list-group :value="true">
            <template v-slot:activator>
              <v-list-item-title>Why Marvel</v-list-item-title>
            </template>
          </v-list-group>
        </v-list-item>
        <v-list-item
          ><v-btn :loading="loading" class="ma-1" color="white" plain
            >Enterprise</v-btn
          ></v-list-item
        >
        <v-list-item
          ><v-btn :loading="loading" class="ma-1" color="white" plain
            >Pricing</v-btn
          ></v-list-item
        >
        <v-list-item
          ><v-btn :loading="loading" class="ma-1" color="white" plain
            >Signin</v-btn
          ></v-list-item
        >
      </v-list>
    </v-navigation-drawer>
    <v-main>
      <MainBody />
    </v-main>
  </v-app>
</template>

<script>
import MainBody from "./components/MainBody";

export default {
  name: "App",

  components: {
    MainBody,
  },

  data: () => ({
    sidebarMenu: false,
  }),
};
</script>
