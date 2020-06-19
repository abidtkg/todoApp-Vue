<template>
    <div>
        <div v-for="todo in todos" v-bind:key="todo.id">
            <TodoItem v-bind:todo="todo" />
        </div>
    </div>
</template>
<script lang="ts">
import Vue from 'vue'
import TodoItem from './TodoItem.vue';
export default Vue.extend({
    name: 'Todos',
    components: {
        TodoItem
    },
    props: ['todos']
})
</script>
<style scoped>

</style>