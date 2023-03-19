<template>
  <div id="app" class="ui container">
    <!-- Notification Message Markup -->
    <!-- Types: info, warning, error, success -->
    <div class="ui message" :class="type" v-if="!hidden">
      <i class="close icon" @click="hide"></i>
      <div class="header">{{ header }}</div>
      <slot />
    </div>
  </div>
</template>

<script>
export default {
  name: "NotificationMessage",
  props: {
    type: String,
    header: String,
  },
  data() {
    return {
      hidden: false,
    };
  },
  methods: {
    hide() {
      this.hidden = true;
    },
  },
};
</script>

<style scoped>
#app {
  margin-top: 1rem;
}
</style>
