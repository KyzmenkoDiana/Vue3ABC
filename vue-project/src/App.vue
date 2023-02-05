<script>
export default {
    data() {
        return {
            cost: 150,
            amount: 7,
        }
    },
    methods: {
        change: function () {
            this.cost = 200;
        },
        change2: function () {
            this.cost = 250;
        }
    },
    computed: {
        price: function () {
            return this.cost * this.amount;
        }
    }
}
</script>

<template>
    <p>{{ price }}</p>
    {{ cost }}
    <button @click="change">cost</button>
    <button @click="change2">cost</button>
</template>

