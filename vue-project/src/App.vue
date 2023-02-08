<script>
import { enableTracking } from '@vue/reactivity';

export default {
    data() {
        return {
            newAvocado: 'Vector',
            Avocado: ['a', 'b', 'c', 'd', 'e'],

        }
    },
    methods: {
        addItem: function () {
            this.Avocado.push(this.newAvocado);
        }
    }
}
</script>

<template>
    <ul>
        <li class="diana" v-for="(item, index) in Avocado" :key="index">
            {{ item }}
        </li>
    </ul>
    <input v-model="newAvocado">
    <button @click="addItem">add</button>
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