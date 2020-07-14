<template>
  <div id="app">
    <RateButton/>
  </div>
</template>

<script>
import RateButton from "@/components/RateButton";

export default {
  name: "App",
  components: {
    RateButton
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 500px;
  height: 200px;
  display: flex;
  flex-direction: column;
}
</style>
