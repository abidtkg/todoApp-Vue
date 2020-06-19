<template>
    <div>
        <h3>{{ todo.id }} . {{ todo.title }} </h3>
    </div>
</template>
<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
    name: 'TodoItem',
    props: ['todo']
})
</script>
<style scoped>

</style>