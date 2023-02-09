<script>
import Avocado from './components/User.vue'
export default {
    components: {
        Avocado
    }
}
</script>

<template>
    <Avocado :arg="{ a: 1, b: 2, c: 3 }" />
</template>
<style>
.diana {
    color: blue;
    font-size: 20px;
}
</style>