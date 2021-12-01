<template>
  <section class="main">
    <GameBar />
    <GameMessages />
    <Buildings />
  </section>
</template>

<script>
import GameBar from './Main/GameBar.vue';
import GameMessages from './Main/GameMessages.vue';
import Buildings from './Main/Buildings.vue';

export default {
  name: 'Main',
  components: {
    GameBar,
    GameMessages,
    Buildings,
  },
  props: {},
};
</script>

<style scoped></style>
