<script setup>
import MiComponente from './MiComponente.vue'

defineProps({
  msg: {
    type: String,
    required: true,
  },
  nombre: {
    type: String,
    required: true,
  },
  apellido: {
    type: String,
    required: true,
  },
});
// export default {
//   name: "HelloWorld",
//   props: {
//     msg2: String,
//   },
//   data() {
//     return {
//       texto: "Hola Mundo Otra VEZ",
//     };
//   }
// };
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h1 class="green">{{ msg }}</h1>
    <p>
      {{ nombre }}<br />
      {{ apellido }}<br />
    </p>
    <MiComponente></MiComponente>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
