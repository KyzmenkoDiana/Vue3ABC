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
        change(id, name, surn) {
            this.users = this.users.map((user) => {
                if (user.id === id) {
                    user.name = name;
                    user.surn = surn;
                }
                return user;
            });
        }
    },
    components: {
        Avocado
    }
}
</script>

<template>
    <Avocado v-for="user in avocados" :id="user.id" :name="user.name" :surn="user.surn" :key="user.id"
        @change="change" />
</template>
<style>
.diana {
    color: blue;
}

.diana1 {
    color: red;
}
</style>