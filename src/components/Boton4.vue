<template>
    <div>
        <button v-bind:style="myStyle">{{ texto }}</button>
    </div>
</template>

<script>
export default {
    name: "BtnIcon",
    data() {
        return {
            texto: "ICON LOADER",
            myStyle: {'backgroundColor':'rgb(18, 52, 114)'}
        }
    },
}
</script>

<style scoped>
/* button{
    background-color: rgb(18, 52, 114);
}

button:hover {
    background-color: rgb(46, 94, 182);
} */
</style>