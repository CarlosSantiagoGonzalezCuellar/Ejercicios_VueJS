<template>
    <div>
        <form @submit.prevent="agregarTarea">
        <input v-model="nuevaTarea" />
        <button>Agregar tarea</button>
        </form>
        <ul>
            <li v-for="tarea in tareas" :key="tarea.id">
            {{ tarea.text }}
            <button @click="eliminarTarea(tarea)">X</button>
            </li>
        </ul>
    </div>
</template>

<script>
let id = 0;

export default {
    name: "ListHomeworks",
    data() {
        return {
        nuevaTarea: "",
        tareas: [],
        };
    },
    methods: {
        agregarTarea() {
        this.tareas.push({ id: id++, text: this.nuevaTarea });
        this.nuevaTarea = "";
        },
        eliminarTarea(tarea) {
        this.tareas = this.tareas.filter((t) => t !== tarea);
        },
    },
};
</script>

<style scoped>
button{
    background-color: rgb(82, 216, 29);
}

button:hover{
    background-color: rgb(58, 173, 47);
}
</style>