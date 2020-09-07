<template>
  <div id="app">
    <section>
      <Top />
      <Mid />
      <Bottom />
    </section>
  </div>
</template>

<script>
import Top from "./components/Top.vue";
import Mid from "./components/Mid.vue";
import Bottom from "./components/Bottom.vue";

export default {
  name: "App",
  components: {
    Top,
    Mid,
    Bottom,
  },
};
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

#app {
  font-family: "Roboto Condensed", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  display: flex;
  justify-content: center;
  background-color: #faf9f7;
}

section {
  background-color: #f3f2ed;
  width: 80em;
}
</style>
