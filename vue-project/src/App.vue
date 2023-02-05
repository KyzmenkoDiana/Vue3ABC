<script>
export default {
    data() {
        return {
            visible1: false,
            visible2: false,
            visible3: false,
        }
    },
    methods: {
        toggle: function () {
            this.visible1 = !this.visible1;
        },
        toggle2: function () {
            this.visible2 = !this.visible2;
        },
        toggle3: function () {
            this.visible3 = !this.visible3;
        }
    }
}

</script>

<template>
    <button @click="toggle">Toggle</button>
    <p v-if="visible1">Hello my name Diana</p>
    <p></p>
    <button @click="toggle2">Toggle2</button>
    <p v-if="visible2">I life in Armyansk</p>
    <p></p>
    <button @click="toggle3">Toggle3</button>
    <p v-if="visible3">Hello world!</p>
</template>

