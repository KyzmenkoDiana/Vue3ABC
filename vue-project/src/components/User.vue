<script>
export default {
    emits: ['show'],
    data() {
        return {
        }
    },

}
</script>

<template>
    <button class="diana" @click="$emit('show', 'Djulietta', '2024')">
        console </button>
</template>