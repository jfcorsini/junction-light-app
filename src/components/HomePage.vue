<template>
  <v-ons-page id="home-page">
    <div class="header">
      <img src="../assets/logo.png" />
    </div>

    <v-ons-list-title>Vue.js Ecosystem</v-ons-list-title>
    <v-ons-row>
      <v-ons-button style="margin: 6px 0">Normal</v-ons-button>
    </v-ons-row>
    <v-ons-row>
      <v-ons-button modifier="quiet" style="margin: 6px 0">Quiet</v-ons-button>
    </v-ons-row>
    <v-ons-row>
      <v-ons-button modifier="outline" style="margin: 6px 0">Outline</v-ons-button>
    </v-ons-row>
    <v-ons-row>
      <v-ons-button modifier="cta" style="margin: 6px 0">Call to action</v-ons-button>
    </v-ons-row>
    <v-ons-row>
      <v-ons-button modifier="large" style="margin: 6px 0">Large</v-ons-button>
    </v-ons-row>
  </v-ons-page>
</template>

<script>
/* eslint-disable */
export default {
  name: "home-page",
  data() {
    return {
      msg: "Welcome",
      essentialLinks: [
        {
          label: "Core Docs",
          link: "https://vuejs.org",
          icon: "fa-book"
        },
        {
          label: "Community Chat",
          link: "https://chat.vuejs.org",
          icon: "fa-commenting"
        },
        {
          label: "Forum",
          link: "https://forum.vuejs.org",
          icon: "ion-chatboxes"
        },
        {
          label: "Twitter",
          link: "https://twitter.com/vuejs",
          icon: "fa-twitter"
        },
        {
          label: "Docs for this template",
          link: "http://vuejs-templates.github.io/webpack/",
          icon: "fa-file-text"
        }
      ]
    };
  },
  methods: {
    goTo(url) {
      window.open(url, "_blank");
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.header {
  text-align: center;
}

img {
  max-width: 300px;
}

ons-list-title {
  text-transform: none;
}

ons-list-title:not(:first-of-type) {
  margin-top: 30px;
}

ons-card {
  text-align: center;
}

ons-list-item,
ons-card {
  cursor: pointer;
}
</style>
