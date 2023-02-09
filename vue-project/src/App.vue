<script>
import Avocado from './components/User.vue'
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
        remove(id) {
            this.avocados = this.avocados.filter((user) => {
                return user.id !== id;
            })
        }
    },
    components: {
        Avocado
    }
}
</script>

<template>
    <Avocado v-for="user in avocados" :id="user.id" :name="user.name" :surn="user.surn" @remove="remove"
        :key="user.id" />
</template>
<style>
.diana {
    color: blue;
}

.diana1 {
    color: red;
}
</style>