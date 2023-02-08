<script>
export default {
    data() {
        return {
            selected: 'Where do you live',
        }
    }
}
</script>

<template>
    <select v-model="selected">
        <option class="diana">Turkish</option>
        <option class="diana1">Russian</option>
        <option class="diana2">USA</option>
    </select>

    <p>{{ selected }}</p>
</template>
<style>
.diana {
    color: blue;
}

.diana1 {
    color: red;
}

.diana2 {
    color: green;
}
</style>