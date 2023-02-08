<script>
export default {
    data() {
        return {
            text: 'Hello Diana',
        }
    }
}
</script>

<template>
    <textarea v-model="text"></textarea>
    <p class="diana">{{ text }}</p>
</template>
<style>
.diana {
    color: blue;
    font-size: 20px;
}
</style>