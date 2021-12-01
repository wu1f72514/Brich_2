<template>
    <!-- Propriétés -->
          <div class="box" for="(item, index) in playerDatas.items">
            <article class="media">
              <div class="media-left">
                <figure class="image is-64x64">
                  <img
                    src="item.img"
                    alt=""
                  />
                </figure>
              </div>
              <div class="media-content">
                <div class="content">
                  <p>
                    <span class="tag is-info" title="Quantité possédée">{ item.owned }</span>
                    <strong>{ item.name }</strong>
                    <br />
                    { item.description }
                    <div class="field is-grouped is-grouped-multiline">
                      <div class="control">
                        <div class="tags has-addons" title="Rendement par tour">
                          <span class="tag is-dark">R <i class="fas fa-dollar-sign"></i></span>
                          <span class="tag is-success">{{item.rendement }</span>
                        </div>
                      </div>
                    
                      <div class="control">
                        <div class="tags has-addons" title="Prix d'achat">
                          <span class="tag is-dark">P <i class="fas fa-dollar-sign"></i></span>
                          <span class="tag is-warning">{item.price }</span>
                        </div>
                      </div>

                      <div class="control">
                        <form>
                          <input class="input buy is-small" type="number" value="1" min="1" max="999" title="Quantité à acheter" />
                        </form>
                        <button class="button is-light is-small" title="Réaliser l'achat" vonclick="buy" data-id="index">Acheter</button>
                        <button class="button is-danger is-light is-small" title="item.owned  0" title="Réaliser la vente" v-on:click="sell" data-id="index">Vendre</button>
                        
                      </div>
                    </div>
                  </p>
                </div>
              </div>
            </article>
  </div>
</template>

<script>
export default {
  name: 'Buildings',
  props: {},
};
</script>

<style scoped></style>
