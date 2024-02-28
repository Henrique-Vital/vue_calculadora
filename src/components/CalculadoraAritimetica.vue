<template>
  <div class="CalculadoraAritimetica">
    <p>Digite o numero mais o operador aritimetico e clique em calcular.</p>
    <input v-model="display" />
    <button @click="calcular()">Calcular</button>    
  </div>
</template>
<script>
export default {
  data() {
    return {
      display: "",
    };
  },
  methods: {
    calcular() {
      try {
        this.display = eval(this.display);
      } catch (error) {
        this.display = "Erro";
      }
    },
  },
};
</script>
