<script>
export default {
    data() {
        return {
            Avocado: ['Djulia', 'vector', 'Flaffi'],
        }
    },
    methods: {
        d: function () {
            this.Avocado.push('Krah');
        },
        i: function () {
            this.Avocado.shift();
        },
        a: function () {
            this.Avocado.pop();
        },
        n: function () {
            this.Avocado.splice(1, 4);
        },
        b: function () {
            this.Avocado.sort();
        },
        g: function () {
            this.Avocado.reverse();
        },
    }
}
</script>

<template>
    <ul>
        <li class="diana" v-for="elem in Avocado">{{ elem }}</li>
    </ul>
    <button class="diana2" @click="add">1</button>
    <br>
    <button class="diana2" @click="d">2</button>
    <br>
    <button class="diana2" @click="a">3</button>
    <br>
    <button class="diana2" @click="n">4</button>
    <br>
    <button class="diana2" @click="b">5</button>
    <br>
    <button class="diana2" @click="g">6</button>
</template>
<style>
.diana {
    color: red;
    font-size: 20px;
}

.diana2 {
    color: blue;
    font-size: 20px;
}
</style>