<template>
  <!-- Compteurs -->
  <div>
    <div class="notification is-danger" if="page.msg.alert.notEnoughCash">
      <button class="delete"></button>
      Vous n'avez pas assez d'argent pour faire cet achat !
    </div>
  </div>
</template>

<script>
export default {
  name: 'GameMessages',
  props: {},
};
</script>

<style scoped></style>
