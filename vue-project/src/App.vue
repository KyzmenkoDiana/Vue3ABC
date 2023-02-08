<script>
export default {
    data() {
        return {
            users: [
                {
                    id: 1,
                    name: 'Vector',
                    salary: 129,
                    age: 38,
                },
                {
                    id: 2,
                    name: 'Djuliet',
                    salary: 250,
                    age: 91,
                },
                {
                    id: 3,
                    name: 'Flaffi',
                    salary: 328,
                    age: 61,
                },
            ]
        }
    },
    methods: {
        edit(user) {
            user.isEdit = true;
        },
        save(user) {
            user.isEdit = false;
        },
    }
}
</script>

<template>
    <table class="diana">
        <tr v-for="user in users" :key="user.id">
            <template v-if="!user.isEdit">
                {{ user.name }}
                {{ user.salary }}
                {{ user.age }}
                <button class="button" @click="edit(user)">edit</button>
            </template>
            <template v-else>
                <input v-model="user.name">
                <input v-model="user.salary">
                <input v-model="user.age">
                <button class="button" @click="save(user)">
                    save
                </button>
            </template>
        </tr>
    </table>
</template>
<style>
.diana {
    color: blue;
}

.diana1 {
    color: red;
}
</style>