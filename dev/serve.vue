<script lang="ts">
import Vue from "vue";
import Player from "@/components/Player.vue";
// @ts-ignore
import { events } from "@/../dev/events";
export default Vue.extend({
  name: "ServeDev",
  components: {
    Player
  },
  data: () => ({
    eventsData: events
  })
});
</script>

<template>
  <div id="app">
    <Player :events="eventsData" />
  </div>
</template>
