<script>
export default {
    props: {
        id: Number,
        name: String,
        surn: String,
    },
    emits: ['remove'],

}
</script>

<template>
    <p class="diana"> {{ name }}</p>
    <p class="diana1">{{ surn }}</p>

    <button @click="$emit('remove', id)">
        delete
    </button>
</template>