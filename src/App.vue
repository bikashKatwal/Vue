<template>
  <div>
    <owt-header></owt-header>
    <owt-content
      channel-name="Oneline Web Tutor"
      name="Bikash Katwal( Default override)"
      :author="{name:'Bikash', email:'bikashkatwal9@gmail.com'}"
      :is-learning="false"
      :myPlaylists="playlists"
    ></owt-content>
    <owt-footer></owt-footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Content from "./components/Content.vue";
import Footer from "./components/Footer.vue";

export default {
  components: {
    "owt-header": Header,
    "owt-content": Content,
    "owt-footer": Footer
  },
  data() {
    return {
      playlists: [
        {
          name: "Wordpress Plugin Development",
          githublink: "https://github.com/owthub/wordpress-plugin",
          title: "Wordpress Plugin Development"
        },
        {
          name: "Wordpress Theme Development",
          githublink: "https://github.com/owthub/wordpress-theme",
          title: "Wordpress Theme Development"
        },
        {
          name: "Vue JS2 Development",
          githublink: "https://github.com/owthub/vuejs2",
          title: "Vue JS2 Development"
        },
        {
          name: "WP JSON Rest API Development",
          githublink: "https://github.com/owthub/wordpress-json-rest-api",
          title: "WP JSON Rest API Development"
        }
      ]
    };
  }
};
</script>

<style>
</style>
