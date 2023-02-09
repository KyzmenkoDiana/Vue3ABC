<script>
export default {
    props: {
        id: Number,
        name: String,
        surn: String,
    },
    emits: ['change'],
    data() {
        return {
            isEdit: false,
            newName: this.name,
            newSurn: this.surn,
        }
    },
    methods: {
        save() {
            this.$emit('change', this.id, this.newName, this.newSurn);
        },
        edit() {
            this.isEdit = true;
        },
    }

}
</script>

<template>
    <template v-if="!isEdit">
        {{ name }}
        {{ surn }}
        <button class="diana" @click="edit">
            edit
        </button>
    </template>
    <template v-else>
        <input v-model="newName">
        <input v-model="newSurn">
        <button class="diana1" @click="save">
            save
        </button>
    </template>
</template>