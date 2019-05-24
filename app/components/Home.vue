<template>
    <div class="big-header">
      <h1>{{ message }}</h1>
      <br />
      <router-link class="button" to="/character">Commencer</router-link>
    </div>
</template>


<script>

export default {
  data() {
    return {
      message: 'Salutations à toi jeune conquérant, l’hiver viens et il faut te préparer à conquérir le trône de fer ! La bataille entre ta maison et tes ennemies sera acharnée prépare toi donc à prendre les bonnes décisions pour pouvoir remporter la victoire !'
    };
  },
  methods: {
    handleClick() {
      countService.increment();
    }
  }
};
</script>


