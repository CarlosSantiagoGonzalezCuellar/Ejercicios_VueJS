<template>
  <div>
    <h1 v-if="cambio">Oprime el boton y cambia el texto!</h1>
    <h1 v-else>Bien! Lo lograste!!</h1>
    <button @click="cambiar">Cambiar texto</button>
  </div>
</template>

<script>
export default {
    name: "ChangeText",
  data() {
    return {
      cambio: true,
    };
  },
  methods: {
    cambiar() {
      this.cambio = !this.cambio;
    },
  },
};
</script>

<style scoped>
button{
    background-color: rgb(85, 160, 231);
}

button:hover {
    background-color: rgb(33, 82, 128);
}
</style>