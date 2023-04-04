<template>
  <div class="boton">
    <button v-bind:style="myStyle">{{ texto }}</button>
  </div>
  <br>
</template>

<script>
export default {
  name: "BtnText",
  props: {
    texto: String,
  },
  data() {
    return {
      myStyle: { backgroundColor: "rgb(228, 115, 23)" },
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* button{
    background-color: rgb(228, 115, 23);
}

button:hover {
    background-color: rgb(165, 80, 10);
} */
</style>
