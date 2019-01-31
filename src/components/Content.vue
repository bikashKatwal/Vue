<template>
  <div>
    <div id="content">
      <h3>Playlists</h3>
      {{ channelName }} - {{ name }}
      <ul>
        <li v-for="playlist in myPlaylists">
          <a :href="playlist.githublink" :title="playlist.title" target="_blank">{{playlist.name}}</a>
        </li>
      </ul>
      {{ call1() }}
    </div>
  </div>
</template>

<script>
export default {
  /* props: ["myPlaylists", "channelName"],*/
  props: {
    name: { type: String, default: " Default Name" },
    channelName: { type: String, required: true },
    myPlaylists: { type: Array },
    author: { type: Object },
    isLearning: { Boolean }
  },
  data() {
    return {
      message: "This is a simple message"
    };
  },
  methods: {
    call1: function() {
      console.log(this.channelName);
    }
  }
};
</script>

<style scoped>
#content {
  text-align: center;
}
#content ul {
  list-style: none;
}
#content ul li {
  font-size: 19px;
  padding: 6px;
  color: #38190e;
}
#content h3 {
  text-align: center;
}
</style>
