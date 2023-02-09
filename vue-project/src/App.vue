<script>
import Avocado from './components/User.vue'
export default {
    data() {
        return {
            name: 'Vector Avocado',
            salary: '9540',
            age: '26',
        }
    },
    components: {
        Avocado
    }
}
</script>

<template>
    <Avocado :name="name" :salary="salary" :age="age" />
</template>
<style>
.diana {
    color: blue;
    font-size: 20px;
}
</style>