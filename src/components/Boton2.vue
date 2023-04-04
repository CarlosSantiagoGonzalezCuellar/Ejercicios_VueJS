<template>
    <div>
        <button v-bind:style="myStyle">{{ texto }} <i class="fas fa-upload"></i></button>
    </div>
</template>

<script>
export default {
    name: "BtnUpload",
    data() {
        return {
            texto: "UPLOAD",
            myStyle: {'backgroundColor':'rgb(73, 89, 104)'}
        }
    },
}
</script>

<style scoped>
/* button{
    background-color: rgb(73, 89, 104);
}

button:hover {
    background-color: rgb(45, 52, 59);
} */
</style>

