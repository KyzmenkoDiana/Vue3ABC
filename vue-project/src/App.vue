<script>
export default {
    data() {
        return {
            age: 25
        }
    }
}

</script>

<template>
    <p class="diana" v-if="age < 18">подросток</p>
    <p class="diana" v-else-if="age > 19 < 25">молодой человек</p>
    <p class="diana" v-else-if="age > 26">мужчина</p>
    <p class="diana" v-else>error</p>
</template>
<style>
.diana {
    color: blue;
    font-size: 30px;
}
</style>
