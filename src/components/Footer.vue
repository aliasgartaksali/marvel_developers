<template>
  <v-footer color="#0b1313" padless>
    <v-row justify="center" no-gutters class="hidden-xs-only">
      <v-col class="ps-3">
        <v-img
          transition="scale-transition"
          alt="Marvel Logo"
          src="../assets/logo-white.svg"
          max-width="200"
          max-height="150"
        />
      </v-col>
      <v-col v-for="item in footerItems" :key="item.name">
        <h3 class="pa-0 ma-0" style="color: white">{{ item.name }}</h3>
        <br />
        <v-container
          class="pa-0 ma-0"
          v-for="content in item.contents"
          :key="content.labelText"
        >
          <h4 style="color: grey">{{ content.labelText }}</h4>
          <br />
        </v-container>
      </v-col>
    </v-row>
    <v-row justify="center" no-gutters class="hidden-sm-and-up">
      <v-col>
        <v-img
          transition="scale-transition"
          alt="Marvel Logo"
          src="../assets/logo-white.svg"
          max-width="100"
          max-height="50"
        />
      </v-col>
    </v-row>
    <v-row justify="center" no-gutters class="hidden-sm-and-up">
      <v-col v-for="item in footerItems" :key="item.name">
        <h3 class="pa-0 ma-0" style="color: white">{{ item.name }}</h3>
        <br />
        <v-container
          class="pa-0 ma-0"
          v-for="content in item.contents"
          :key="content.labelText"
        >
          <h4 style="color: grey">{{ content.labelText }}</h4>
          <br />
        </v-container>
      </v-col>
    </v-row>
  </v-footer>
</template>

<script>
export default {
  data: () => ({
    footerItems: [ // used as data for footer. done using for loop
      {
        name: "Overview",
        contents: [
          {
            labelText: "Why Marvel",
          },
          {
            labelText: "Enterprise",
          },
          {
            labelText: "Pricing",
          },
          {
            labelText: "Request a demo",
          },
          {
            labelText: "Explore",
          },
          {
            labelText: "Apps",
          },
          {
            labelText: "Developer API",
          },
        ],
      },
      {
        name: "Features",
        contents: [
          {
            labelText: "Wireframing",
          },
          {
            labelText: "Design",
          },
          {
            labelText: "Prototyping",
          },
          {
            labelText: "Collaboration",
          },
          {
            labelText: "Handoff",
          },
          {
            labelText: "Integrations",
          },
          {
            labelText: "Sketch Plugin",
          },
        ],
      },
      {
        name: "Support",
        contents: [
          {
            labelText: "Help Center",
          },
          {
            labelText: "Terms of Service",
          },
          {
            labelText: "Privacy",
          },
          {
            labelText: "Security",
          },
        ],
      },
      {
        name: "Marvel",
        contents: [
          {
            labelText: "Blog",
          },
          {
            labelText: "Our Team",
          },
          {
            labelText: "Contact Us",
          },
          {
            labelText: "Success Stories",
          },
          {
            labelText: "Brand Guidelines",
          },
        ],
      },
    ],
  }),
};
</script>

<style>
</style>