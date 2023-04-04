<template>
<div>
    <input v-model="text" placeholder="Escribe aqui..." />
    <p>{{ text }}</p>
</div>
</template>

<script>
export default {
    name: "FormText",
  data() {
    return {
      text: "",
    };
  },
};
</script>