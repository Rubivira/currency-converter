<template>
  <div class="app">
    <h1 class="title">Conversor de Moedas</h1>
    <div class="linha">
      <Conversor moeda-a="USD" moeda-b="BRL" />
      <Conversor moeda-a="BRL" moeda-b="USD" />
    </div>
    <div class="linha">
      <Conversor moeda-a="CAD" moeda-b="BRL" />
      <Conversor moeda-a="BRL" moeda-b="CAD" />
    </div>
    <div class="linha">
      <Conversor moeda-a="EUR" moeda-b="BRL" />
      <Conversor moeda-a="BRL" moeda-b="EUR" />
    </div>
  </div>
</template>

<script>
import Conversor from "./components/Conversor.vue";
export default {
  name: "App",
  components: {
    Conversor,
  },
};
</script>

<style>
.app {
  max-width: 900px;
  margin: auto;
  margin-top: 60px;
  font-family: "Avenir, Helvetica, Arial", sans-serif;
  color: #2c3e50;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  
}

.linha {
  margin-top: 40px;
  display: flex;
  justify-content: space-around;
}

.title {
  text-align: center;
}
</style>
