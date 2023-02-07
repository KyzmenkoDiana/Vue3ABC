<script>
export default {
    data() {
        return {
            diana: true,
        }
    },
    methods: {
        Diana: function () {
            this.diana = false;
        }
    }
}
</script>

<template>
    <button @click="Diana">diana</button>
    <div v-if="diana">
        <p class="diana">Djulia</p>
        <p class="diana1">Vector</p>
        <p class="diana2">Flaffi</p>
    </div>
</template>
<style>
.diana {
    color: blue;
    font-size: 30px;
}

.diana1 {
    color: red;
    font-size: 30px;
}

.diana2 {
    color: yellow;
    font-size: 30px;
}
</style>
