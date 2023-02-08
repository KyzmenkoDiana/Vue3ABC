<script>
export default {
    data() {
        return {
            users: [
                {
                    id: 1,
                    name: 'vector',
                    salary: 100,
                    age: 30,
                },
                {
                    id: 2,
                    name: 'Flaffi',
                    salary: 200,
                    age: 40,
                },
                {
                    id: 3,
                    name: 'Djuliya',
                    salary: 300,
                    age: 50,
                },
                methods: {
                    Diana: function (id) {
                        this.users = this.users.filter((user) => {
                            return user.id !== id;
                        })
                    }
                }
    }
    }
}
</script>

<template>
    <table class="diana">
        <ul>
            <li v-for="user in users" :key="user.id">
                {{ user.name }}
                {{ user.salary }}
                {{ user.age }}
                <button @click="Diana(user.id)">delete</button>
            </li>
        </ul>
    </table>
</template>
<style>
.diana {
    color: blue;
}
</style>