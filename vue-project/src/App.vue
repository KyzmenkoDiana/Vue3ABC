<script>
export default {
    data() {
        return {
            day: 5
        }
    }
}

</script>

<template>
    <p class="diana" v-if="day === 1">понедельник</p>
    <p class="diana" v-if="day === 2">вторник</p>
    <p class="diana" v-if="day === 3">среда</p>
    <p class="diana" v-if="day === 4">четверг</p>
    <p class="diana" v-if="day === 5">пятница</p>
    <p class="diana" v-if="day === 6">суббота</p>
    <p class="diana" v-if="day === 7">воскресенье</p>
</template>
<style>
.diana {
    color: blue;
    font-size: 30px;
}
</style>
