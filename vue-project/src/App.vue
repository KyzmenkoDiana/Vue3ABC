<script>
export default {
    data() {
        return {
            isDisabled: true,
            open: true,
            checked: false,
        }
    },
    methods: {
        toggle: function () {
            this.isDisabled = !this.isDisabled;
        }
    }
}
</script>

<template>

    <button class="diana" @click="toggle">Hello</button>
    <button v-bind:disabled="isDisabled">Hello</button>
    <button v-bind:disabled="checked">Good bay</button>
    <input type="checkbox" v-model="checked" @click="clic">
</template>
<style>
.diana {
    color: blue;
}

.diana1 {
    color: red;
}

.diana2 {
    color: rebeccapurple;
}
</style>