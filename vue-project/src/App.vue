<script>
export default {
    data() {
        return {
            hidden1: false,
        }
    },
    methods: {
        hide: function () {
            this.hidden1 = true;
        },
        hide2: function () {
            this.hidden1 = false;
        }
    }
}

</script>

<template>
    <p v-if="hidden1">Hello my name is Diana</p>
    <button @click="hide">Нажми</button>
    <button @click="hide2">Упсс</button>
</template>

