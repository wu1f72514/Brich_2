<template>
  <!-- Compteurs -->
  <nav class="level">
    <div class="level-item has-text-centered">
      <div class="tags has-addons" title="Rendement total par tour">
        <span class="tag is-dark"> R <i class="fas fa-dollar-sign"></i></span>
        <span class="tag is-success">{ playerDatas.moneyRendement }</span>
      </div>
    </div>
    <div class="level-item has-text-centered">
      <div class="tags has-addons" title="Trésorerie">
        <span class="tag is-dark"> <i class="fas fa-dollar-sign"></i></span>
        <span class="tag is-info">{ playerDatas.moneyCapital }</span>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'GameBar',
  props: {},
};
</script>

<style scoped></style>
