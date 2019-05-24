<template>
  <div class="big-header">
    <h1>{{message}}</h1>
    <br />
    <router-link class="button" to="/game/1">Lannister</router-link>
    <br />
    <router-link class="button" to="/game/2">Targaryen</router-link>
  </div>
</template>

<script>

export default {
  data() {
    return {
      message: 'Quel maison choisis-tu ?'
    }
  }
};
</script>
