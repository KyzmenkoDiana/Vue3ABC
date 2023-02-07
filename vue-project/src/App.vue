<script>
export default {
    data() {
        return {
            num: 6,
            res: 0,
            sum: 0,
            num1: 11,
            num2: 8,
            d: 'Hello',
            d1: 'world',
        }
    },
    methods: {
        Diana: function () {
            this.res = Math.sqrt(this.num);
        },
        summary: function () {
            this.sum = this.num1 + this.num2;
        },
        vector: function () {
            this.d = this.d1;

        }
    }
}
</script>

<template>
    <p class="diana">{{ res }}</p>
    <input class="diana1" v-model="num">
    <button class="diana2" @click="Diana">квадратный корень</button>
    <br>
    <p class="diana">{{ sum }}</p>
    <input class="diana1" v-model=num1>
    <input class="diana1" v-model=num2>
    <button class="diana2" @click="summary">сумма</button>
    <br>
    <input class="diana1" v-model=d>
    <input class="diana1" v-model=d1>
    <button class="diana2" @click="vector">обмен</button>
</template>
<style>
.diana {
    color: blue;
    font-size: 20px;
}

.diana1 {
    color: red;
    font-size: 20px;
}

.diana2 {
    color: green;
    font-size: 20px;
}
</style>