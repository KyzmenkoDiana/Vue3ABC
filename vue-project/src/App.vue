<script>
export default {
    data() {
        return {
            selected: 'data',
            options: ['1', '2', '3', '4', '5', '6', '7'],
            selected1: 'month',
            options1: ['январь', 'февраль', 'март', 'апрель', 'май', 'июнь', 'июль'],
            selected2: 'year',
            options2: ['20014', '2015', '2016', '2017', '2018', '2019', '2020'],
        }
    }
}
</script>

<template>
    <select v-model="selected">
        <option class="diana" v-for="option in options">{{ option }}</option>
    </select>
    <p>{{ selected }}</p>
    <b></b>
    <select v-model="selected1">
        <option class="diana1" v-for="option in options1">{{ option }}</option>
    </select>
    <p>{{ selected1 }}</p>
    <b></b>
    <select v-model="selected2">
        <option class="diana2" v-for="option in options2">{{ option }}</option>
    </select>
    <p>{{ selected2 }}</p>
</template>
<style>
.diana {
    color: blue;
}

.diana1 {
    color: red;
}

.diana2 {
    color: rebeccapurple;
}
</style>