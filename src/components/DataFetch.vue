<template>
    <div>
        <p>ID Dato: {{ todoId }}</p>
        <button @click="todoId++">Siguiente dato</button>
        <p v-if="!todoData">Cargando...</p>
        <pre v-else>{{ todoData }}</pre>
    </div>
</template>

<script>
export default {
    name: "DataFetch",
    data() {
        return {
        todoId: 1,
        todoData: null
        }
    },
    methods: {
        async fetchData() {
        this.todoData = null
        const res = await fetch(
            `https://jsonplaceholder.typicode.com/todos/${this.todoId}`
        )
        this.todoData = await res.json()
        }
    },
    mounted() {
        this.fetchData()
    },
    watch: {
        todoId() {
        this.fetchData()
        }
    }
}
</script>

<style scoped>
button{
    background-color: darkorange;
}

button:hover{
    background-color: rgb(156, 90, 8);
}
</style>
