<template>
  <div class="big-header">
    <h1>{{step.title}}</h1>
    <br />
    <router-link v-for="answer in answers" v-bind:key="answer.message" class="button" :to="answer.link">{{answer.message}}</router-link>
  </div>
</template>

<script>
import data from '../data.json';

export default {
  data() {
      return{
        step : data.steps[this.$route.params.id],
        answers: data.steps[this.$route.params.id].answers
      }
  }
};
</script>