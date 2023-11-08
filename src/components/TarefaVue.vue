<template>
    <Box>
      <div class="columns">
        <div class="column is-7">{{ tarefa.descricao || 'Tarefa sem descrição' }}</div>
        <div class="column">
          <Cronometro :tempoEmSegundos="tarefa.duracaoEmSegundos"/>
        </div>
      </div>
    </Box>
  </template>
  
  <script lang="ts">
  import { defineComponent, PropType } from "vue";
  import Cronometro from "./CronometroVue.vue";
  import ITarefa from '../ITarefa'
  import Box from './BoxVue.vue'
  
  export default defineComponent({
    name: "TarefaVue",
    components: {
      Cronometro,
      Box
    },
    props: {
      tarefa: {
        type: Object as PropType<ITarefa>,
        required: true
      }
    }
  });
  </script>../ITarefa