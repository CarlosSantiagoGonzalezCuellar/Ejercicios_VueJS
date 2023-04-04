<template>
    <div>
        <button v-bind:style="myStyle">{{ texto }}</button>
    </div>
</template>

<script>
export default {
    name: "BtnAccept",
    data() {
        return {
            texto: "ACCEPT TERMS",
            myStyle: {'backgroundColor':'rgb(85, 160, 231)'}
        }
    },
}
</script>

<style scoped>
/* button{
    background-color: rgb(85, 160, 231);
}

button:hover {
    background-color: rgb(33, 82, 128);
} */
</style>