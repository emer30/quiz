<template>
    <ion-input v-bind="$attrs" :Type ="type" :id="id" :value="value" :placeholder="placeholder" :clearInput="clearInput" :debounce="debounce" :disabled="disabled" :maxlength="maxlength" :min="min" :max="max" :step="step"></ion-input>
  </template>
  
  <script lang="ts">
  import { IonInput } from '@ionic/vue';
  import { defineComponent } from 'vue';

  
  
  export default defineComponent({
    components: { IonInput },
    props: {
       type : String,
      id: {
        type: String,
        required: true
      },name: String,
      value: String,
      placeholder: String,
      clearInput: Boolean,
      debounce: Number,
      disabled: Boolean,
      maxlength: Number,
      min: Number,
      max: Number,
      step: String,
    }
  });
  </script>
  
  <style scoped>
  /* Estilos del componente */
  /* Estilos globales */
  </style>