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
        diana1(name, age) {
            console.log(name, age);
        }
    }
}
</script>

<template>
    <Avocado @show="diana1" />
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