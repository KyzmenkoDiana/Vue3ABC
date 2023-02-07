<script>
export default {
    data() {
        return {
            items: [1, 2, 3, 4, 5],
        }
    }
}
</script>

<template>
    <div class="diana" v-for="elem in items">{{ elem }}</div>
    <p></p>
    <p></p>
    <div class="diana" v-for="elem in items">{{ elem*elem }}</div>
    <p></p>
    <ul class="diana" v-for="elem in items">{{ elem }}</ul>
</template>
<style>
.diana {
    color: blue;
    font-size: 20px;
}
</style>
