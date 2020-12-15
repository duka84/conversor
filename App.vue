<template>
  <div id="app">
    <h1 class="text-center">Conversor de Moedas</h1>
    <div class="linha">
    <Conversor moeda-a="USD" moeda-b="BRL"/>
     <Conversor moeda-a="CAD" moeda-b="BRL"/>
    </div>
    <div class="linha">
    <Conversor moeda-a="EUR" moeda-b="BRL"/>
    <Conversor moeda-a="GBP" moeda-b="BRL"/>
    </div>
    <div class="linha">
    <Conversor moeda-a="ARS" moeda-b="BRL"/>
    <Conversor moeda-a="CHF" moeda-b="BRL"/>
    </div>
  </div>
</template>

<script>
import Conversor from "./components/Conversor.vue";
export default {
  name:"app",
  components: {
    Conversor
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
   color: #2c3e50;
  margin-top: 60px;
}
.linha{
  margin-top: 40px;
  display: flex;
  justify-content: space-around;
}
.text-center{
  text-align: center;
}
</style>
