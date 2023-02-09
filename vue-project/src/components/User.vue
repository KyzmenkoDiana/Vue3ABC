<script>
export default {
    data() {
        return {
            newName: '',
            newSurn: '',
        }
    },
    methods: {
        save() {
            this.$emit('add', this.newName, this.newSurn);
        }
    }
}
</script>

<template>
    <input v-model="newName">
    <input v-model="newSurn">
    <button class="diana" @click="save">save</button>
</template>