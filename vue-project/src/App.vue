<script>
export default {
    data() {
        return {
            diana: [1, 2, 3],
        }
    }
}
</script>

<template>
    <div v-for="elem in diana">
        <p class="divider">{{ elem }}</p>
    </div>
    <b>
    </b>
    <ul v-for="elem in diana">
        <li class="divider">{{ elem }}</li>
    </ul>
</template>
<style>
.divider {
    color: blue;
    font-size: 20px;
}
</style>