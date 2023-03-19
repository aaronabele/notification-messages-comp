<template>
  <h1>Notification Center</h1>
  <NotificationMessage type="error" header="Oh no!">
    <p>Your flight has been <b>canceled</b></p>
  </NotificationMessage>

  <NotificationMessage type="success" header="Oh yeah!">
    <p>Your flight is on time!</p>
  </NotificationMessage>

  <NotificationMessage type="info" header="Good morning!">
    <p>HAVE A NICE DAY</p>
  </NotificationMessage>
</template>

<script>
import NotificationMessage from "./components/NotificationMessage.vue";

export default {
  name: "App",
  components: {
    NotificationMessage,
  },
};
</script>

<style></style>
