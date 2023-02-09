<script>
import AvocadoForm from './components/User.vue'
export default {
    data() {
        return {
            avocados: [
                {
                    id: 1,
                    name: 'Vector',
                    surn: 'Avocado'
                },
                {
                    id: 2,
                    name: 'Djuliet',
                    surn: 'Avocado'
                },
                {
                    id: 3,
                    name: 'Flaffi',
                    surn: 'Avocado'
                },
            ],
        }
    },
    methods: {
        add(name, surn) {
            let id = this.avocados.length + 1;
            this.avocados.push({
                id,
                name,
                surn
            });
        }
    },
    components: {
        AvocadoForm
    }
}
</script>

<template>
    <AvocadoForm @add="add" />
</template>
<style>
.diana {
    color: blue;
}
</style>