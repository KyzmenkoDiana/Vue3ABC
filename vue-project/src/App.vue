<script>
export default {
    data() {
        return {
            products: [
                {
                    id: 1,
                    name: 'Djuliet',
                },
                {
                    id: 2,
                    name: 'Vector',
                },
                {
                    id: 3,
                    name: 'Flaffi',
                },
            ]
        }
    }
}
</script>

<template>

    <ul class="diana" v-for="user in products" :key="user.id">
        {{ user.name }}
    </ul>
</template>
<style>
.diana {
    color: red;
    font-size: 20px;
}
</style>