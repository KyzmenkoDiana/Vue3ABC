<script>
export default {
    data() {
        return {
            items: [1, -2, 3, -4, 5],
        }
    }
}
</script>

<template>
    <ul>
        <template v-for="elem in items">
            <li class="diana" v-if="elem > -1">
                {{ elem }}
            </li>
        </template>
    </ul>
</template>
<style>
.diana {
    color: red;
    font-size: 20px;
}
</style>