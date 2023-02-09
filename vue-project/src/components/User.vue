<script>
export default {
    emits: ['show', 'show1'],
    data() {
        return {
        }
    },
    methods: {
        diana() {
            this.$emit('show');
        },
        diana1() {
            this.$emit('show1');
        },
    }
}
</script>

<template>
    <button class="diana" @click="diana">Name</button>
    <button class="diana1" @click="diana1">Data</button>
</template>