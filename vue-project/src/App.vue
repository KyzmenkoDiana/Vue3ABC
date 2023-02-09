<script>
import Avocado from './components/User.vue'

export default {
    data() {
        return {
            diana: [
                {
                    id: 1,
                    name: 'Djuliet',
                    salary: 730,
                    age: 20,
                },
                {
                    id: 2,
                    name: 'Vector',
                    salary: 1000,
                    age: 26,
                },
                {
                    id: 3,
                    name: 'Flaffi',
                    salary: 300,
                    age: 10,
                }
            ]
        }
    },
    components: {
        Avocado
    }
}
</script>

<template>
    <Avocado v-for="Avocado in diana" :name="Avocado.name" :salary="Avocado.salary" :age="Avocado.age"
        :key="Avocado.id" />
</template>
<style>
.diana {
    color: blue;
    font-size: 20px;
}
</style>