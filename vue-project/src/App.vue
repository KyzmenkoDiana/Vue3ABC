<script>
export default {
    data() {
        return {
            message: 'Diana Kuzmenko',
            number: '45',
        }
    }
}
</script>

<template>
    <input class="diana" v-model="message">
    <p :style="{ textTransform: 'uppercase' }">{{ message }}</p>
    <br>
    <input class="diana" v-model="number">
    <p>{{ number*number }}</p>
</template>
<style>
.diana {
    color: blue;
    font-size: 20px;
}
</style>