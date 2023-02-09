<script>
import Avocado from './components/User.vue'
export default {
    data() {
        return {

        }
    },
    components: {
        Avocado
    },
    methods: {
        name() {
            alert('Vector Avocado');
        },
        data() {
            alert('09.02.2023')
        }
    }
}
</script>

<template>
    <Avocado @show="name" @show1="data" />
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