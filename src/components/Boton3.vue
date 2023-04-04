<template>
    <div>
        <button v-bind:style="myStyle">{{ texto }}</button>
    </div>
</template>

<script>
export default {
    name: "BtnCustom",
    data() {
        return {
            texto: "CUSTOM LOADER",
            myStyle: {'backgroundColor':'rgb(37, 145, 46)'}
        }
    },
}
</script>

<style scoped>
/* button{
    background-color: rgb(37, 145, 46);
}

button:hover {
    background-color: rgb(67, 209, 79);
} */
</style>