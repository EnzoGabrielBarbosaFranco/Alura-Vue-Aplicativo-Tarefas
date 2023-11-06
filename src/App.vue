<template>
  <main class="columns is-gapless is-multiline">
    <div class="column is-one-quarter">
      <BarraLateral/>
    </div>
    <div class="column is-three-quarter">
      <FormularioVue/>
    </div>
  </main>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import BarraLateral from './components/BarraLateral.vue';
import FormularioVue from './components/FormularioVue.vue';


export default defineComponent({
    name: 'App',
    components: { 
      BarraLateral,
      FormularioVue 
    }
});
</script>

<style></style>
