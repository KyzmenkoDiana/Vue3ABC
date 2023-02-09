<script>
export default {
    emits: ['show', 'show1'],
    data() {
        return {
        }
    },
    methods: {
        diana() {
            this.$emit('show', 'Vector', '8352');
        },
        diana1() {
            this.$emit('show1', 'Vector');
        }
    }
}
</script>

<template>
    <button class="diana" @click="diana">console</button>
    <button class="diana" @click="diana1">console1</button>
</template>