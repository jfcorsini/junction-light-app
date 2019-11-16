<template>
  <v-ons-page id="light-page">
    <v-ons-list-title>This is the light page!</v-ons-list-title>
  </v-ons-page>
</template>

<script>
/* eslint-disable */
export default {
  name: "light-page",
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
