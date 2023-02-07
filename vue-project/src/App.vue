<script>
export default {
    data() {
        return {
            arr: ['x', 'y', 'z'],
        }
    }
}
</script>

<template>
    <ul v-for="(elem, key) in arr">
        {{ key }} {{ elem }} </ul>
</template>
<style>
.diana {
    color: blue;
    font-size: 20px;
}
</style>
