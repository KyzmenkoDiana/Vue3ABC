<script>

export default {
    data() {
        return {
            a: 'Vector',
            b: 'Flaffi',
            c: 'Djuliet',
            Avocado: true,
        }
    },
    methods: {
        Diana() {
            alert('Avocado');
        },
    }
}
</script>

<template>
    <!--В этом задании был только текст. Прочитала, ознакомилась.-->
    <button class="diana" @click="Diana">Avocado</button>
    <br>
    <p class="diana1">{{ a }}</p>
    <br>
    <p class="diana2">{{ b }}</p>
    <br>
    <p class="diana3">{{ c }}</p>
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
    color: yellow;
    font-size: 20px;
}

.diana3 {
    color: green;
    font-size: 20px;
}
</style>