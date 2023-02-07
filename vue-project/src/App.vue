<script>
export default {
    data() {
        return {
            Diana: { user1: '100$', user2: '200$', user3: '300$' },
        }
    }
}
</script>

<template>
    <ul>
        <li v-for="elem in Diana">{{ elem }}</li>
    </ul>
    <b>
    </b>
    <ul>
        <li v-for="(key, elem) in Diana"> {{ elem }} - {{ key }}</li>
    </ul>
    <b>
    </b>
    <ul>
        <li v-for="(key, elem, index) in Diana"> {{ elem }} - {{ key }} - {{ index }}</li>
    </ul>
    <b>
    </b>
    <ul>
        <li v-for="(key, elem, index) in Diana"> {{ elem }} - {{ key }} - {{ index+ 1 }}</li>
    </ul>
</template>
