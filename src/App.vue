<template>
  <div id="app">
    <h1>Conversor de Moedas</h1>
    <div class="linha">
      <Conversor moeda-a="USD" moeda-b="BRL"></Conversor>
      <Conversor moeda-a="BRL" moeda-b="USD"></Conversor>
    </div>
      <div class="linha">
      <Conversor moeda-a="CAD" moeda-b="BRL"></Conversor>
      <Conversor moeda-a="BRL" moeda-b="CAD"></Conversor>
    </div>
  </div>
</template>

<script>
import Conversor from "./components/Conversor";

export default {
  name: 'App',
  components: {
    Conversor,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  max-width: 800px;
}

.linha{
  display: flex;
  justify-content: space-between;
  margin-top: 30px;
}
</style>
