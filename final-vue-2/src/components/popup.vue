<template>
    <div>
        <h2>This is popup</h2>
        <button @click="$emit('close')">Close the friking popup!</button>
    </div>
</template>

<script>
    export default {
        name: 'mi-popup',
        emits: ['close']
    }
</script>

<style scoped>

</style>