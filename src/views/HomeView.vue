<script setup lang="ts">
import { ref, onMounted } from 'vue';

const todos = ref([])

const createTodo = () => ({

})

</script>

<template>
    <div class="header">
        <h1>Effinote - made by Qbi for Linus :)</h1>
    </div>
    <div class="main">
        <div class="todo">
            <div class="todo-add">
                <input class="todo-input" type="text">
                <button 
                    class="todo-create"
                    @click="createTodo"
                >Add
                </button>
            </div>
            <div class="todo-list">
                <ul class="todos">

                </ul>
            </div>
        </div>        
    </div>
</template>

<style scoped>

h1 {
    text-align: center;
}

ul {
    list-style: none;
    margin: 0;
    padding: 0;
}

input:focus {
    outline: none;
}

.main {
    display: flex;
    align-items: center;
    text-align: center;
    justify-content: center;
}

.todo {
    padding: 10px;
    margin: 0;
    width: 400px;
    height: 600px;
    background-color: #222;
    border: #333 solid 2px;
    border-radius: 2%;
}

.todo-list {
    width: 100%;
    height: 95%;
    background-color: #444;
}

.todo-add {
    width: 100%;
    height: 5%;
    display: flex;
    justify-content: center;
    align-items: center;
}

.todo-create {
    border-radius: 4%;
    margin: 2px;
    background-color: #333;
    border: none;
    width: 20%;
}

.todo-create:hover {
    background-color: #38ce38;
    color: #000;
    border-radius: 4%;
    border: none;
}

.todo-input {
    width: 80%;
    margin: 2px;
    border: none;
    background-color: #333;
}

</style>