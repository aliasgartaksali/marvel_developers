<template>
  <v-container class="backgroundcolor">
    <v-row>
      <v-col>
        <v-row>
          <h1 style="color: white">Let's build the future of design, now.</h1>
        </v-row>
        <v-row>
          <p style="color: white">Create amazing tools and integrations for 1 million users or customise Marvel for your team.</p>
        </v-row>
        <v-row>
          <v-col>
            <v-btn rounded color="blue" dark class="white--text">Submit your app</v-btn>
          </v-col>
          <v-col>
            <v-btn rounded color="white" dark class="black--text">View API Docs</v-btn>
          </v-col>
        </v-row>
      </v-col>
      <v-col>
        <v-img alt="Illustration" src="../assets/illustration.png" />
      </v-col>
    </v-row>
    <h2 style="color: white">Experience the freedom to build features, right away.</h2>
    <p style="color: white">You can now harness components of our platform and build powerful integrations for our 2 million users - or simply just for your team.</p>
    <v-row>
      <v-col>
        <v-row>
          <v-img alt="Illustration" src="../assets/apiTeam@2x-5a72bbd0df3f17c4851dca773b2b1b8f-3ad8f.png" />
        </v-row>
        <v-row>
          <h3 style="color: white">Dedicated API Team</h3>
        </v-row>
        <v-row>
          <p style="color: grey">Our team are available for user's questions via our Slack Developer Community and Email</p>
        </v-row>
      </v-col>
      <v-col>
        <v-row>
          <v-img alt="Illustration" src="../assets/graphQL.png" />
        </v-row>
        <v-row>
          <h3 style="color: white">Our API uses Graph QL</h3>
        </v-row>
        <v-row>
          <p style="color: grey">No handling server side. Get many API's responses in a single request.</p>
        </v-row>
      </v-col>
      <v-col>
        <v-row>
          <v-img alt="Illustration" src="../assets/superchargeWorkflow.png" />
        </v-row>
        <v-row>
          <h3 style="color: white">Supercharge your workflow</h3>
        </v-row>
        <v-row>
          <p style="color: grey">Automate workflows, integrate and analyse data and take Marvel to the next level.</p>
        </v-row>
      </v-col>
    </v-row>
    <v-row>
      <v-col>
        <h1 style="color: white">Showcase your app in our integrations directory</h1>
        <p style="color: white">Building something special? We're always looking to work with partners who wants to help the world bring their ideas to life.</p>
        <v-col><v-btn rounded color="white" dark class="black--text">Become a partner</v-btn></v-col>
        <v-col><v-btn rounded color="black" dark class="white--text">View Integrations</v-btn></v-col>
      </v-col>
      <v-col>
        <v-img alt="Illustration" src="../assets/showcase.png" />
      </v-col>
    </v-row>
    <v-row>
      <v-col>
        <v-img alt="Illustration" src="../assets/botbot.png" />
      </v-col>
      <v-col>
        <h1 style="color: white">A Slack-bot for creating and managing prototypes</h1>
        <p style="color: white">Building something special? We're always looking to work with partners who wants to help the world bring their ideas to life.</p>
        <v-col><v-btn rounded color="white" dark class="black--text">Become a partner</v-btn></v-col>
        <v-col><v-btn rounded color="black" dark class="white--text">View Integrations</v-btn></v-col>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
    name: 'MainBody',
    data: () => ({
        //
    })
};
</script>

<style scoped>
.backgroundcolor {
  background-color: #0b1313;
}
</style>