<template>
  <div>
    <h1>Este es mi componente</h1>
    <h2>{{subtitulo}}</h2>
  </div>
</template>

<script>
export default {
  name: "MiComponente", 
  data() {
    return {
      subtitulo: "Soy el subtituto de mi componente",
    };
  },
};
</script>
