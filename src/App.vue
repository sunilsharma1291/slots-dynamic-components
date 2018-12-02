<template>
  <div id="app">
    <app-quote>
        <h2 slot="quotetitle">{{ quoteTitle }}</h2>
        <p slot="quotedesc">{{ quoteHeading }}</p>
        <p>This can be considered as default slot and would be available as non naming slots</p>
    </app-quote>

    <hr>
    <dynamic-component></dynamic-component>    
  </div>
</template>

<script>
import Quote from "./components/Quote.vue";
import DynamiccomponentVue from './components/Dynamiccomponent.vue';

export default {
  name: "app",
  data() {
    return {
      quoteTitle: "The Quote",
      quoteHeading: `This can be total text written.`
    };
  },

  components: {
    "app-quote": Quote,
    "dynamic-component": DynamiccomponentVue
  }
};
</script>

<style>
</style>
