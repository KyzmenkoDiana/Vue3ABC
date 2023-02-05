<script>
export default {
    data() {
        return {
            visible1: true,
            visible2: false,
        }
    }
}

</script>

<template>
    <p v-if="visible1">Hello my name Diana</p>
    <h1></h1>
    <p v-if="visible2">I life in Armyansk</p>
</template>

