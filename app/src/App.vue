<template>
  <div class="container grid-lg">
    <input v-model="model" />
    <h1>{{ model }}</h1>
  </div>
</template>

<script>
import { ref } from "vue";
export default {
  name: "App",
  setup() {
    
    //usando o ref, aplica reatividade no input conforme apaga ou digita o texto
    const model = ref("Teste usando o setup");
    return { model };
  },
};
</script>


