<template>
  <v-ons-page id="app">
    <v-ons-splitter>
      <v-ons-splitter-content>
        <v-ons-tabbar
          swipeable
          position="auto"
          :tabs="tabs"
          :visible="true"
          :index.sync="activeIndex"
        ></v-ons-tabbar>
      </v-ons-splitter-content>
    </v-ons-splitter>
    <!-- <ons-tabbar swipeable position="auto">
      <ons-tab page="tab1.html" label="Tab 1" icon="ion-home, material:md-home" badge="7" active></ons-tab>
      <ons-tab page="tab2.html" label="Tab 2" icon="md-settings" active-icon="md-face"></ons-tab>
    </ons-tabbar>-->
  </v-ons-page>
</template>



<script>
/* eslint-disable */
import HomePage from "./components/HomePage";
import LightPage from "./components/LightPage";
import MoodPage from "./components/MoodPage";

export default {
  name: "app",

  components: {
    LightPage,
    HomePage,
    MoodPage
  },

  data() {
    return {
      activeIndex: 0,
      tabs: [
        {
          label: "Home",
          page: HomePage,
          props: {
            myProp: "This is a page prop!"
          },
          key: "homePage"
        },
        {
          label: "Light",
          page: LightPage,
          // badge: 7,
          key: "lightPage"
        },
        {
          label: "Mood",
          page: MoodPage,
          key: "moodPage"
        }
      ]
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
ons-splitter-side[side="left"][animation="overlay"] {
  border-right: 1px solid #bbb;
}
</style>
