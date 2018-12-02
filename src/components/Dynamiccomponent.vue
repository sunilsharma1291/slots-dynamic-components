<template>
  <div class="dynamic-component-panel">
    <h2>To study dynamic components</h2>
    <button @click="selectedComponent = 'Blue'">blue slide</button>
    <button @click="selectedComponent = 'Green'">green slide</button>
    <button @click="selectedComponent = 'Red'">red slide</button>

    <div>
        <keep-alive>
            <component :is="selectedComponent"></component>
        </keep-alive>
      
    </div>
  </div>
</template>

<script>
import Blue from "./Blue.vue";
import Green from "./Green.vue";
import Red from "./Red.vue";

export default {
  data() {
    return {
      selectedComponent: "Blue"
    };
  },
  components: {
    Blue: Blue,
    Green: Green,
    Red: Red
  }
};
</script>

<style>
.dynamic-component-panel {
  color: #333;
  text-align: center;
  margin-top: 20px;
}
div {
  padding: 10px 0;
}
</style>