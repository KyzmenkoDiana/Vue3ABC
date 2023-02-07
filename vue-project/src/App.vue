<script>
export default {
    data() {
        return {
            visible: true,
            visible2: true,
            visible3: true
        }
    },
    methods: {
        toggle: function () {
            this.visible = !this.visible;
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
    <button class="clic" @click="toggle">toggle</button>
    <p class="diana">{{ visible? 'Avocado': 'Julia' }}</p>
    <button class="clic" @click="toggle2">toggle</button>
    <p class="diana1">{{ visible2? 'Avocado': 'Vector' }}</p>
    <button class="clic" @click="toggle3">toggle</button>
    <p class="diana2">{{ visible3? 'Avocado': 'Flaffi' }}</p>
</template>
<style>
.diana {
    color: blue;
    font-size: 30px;
}

.clic {
    color: black;
    font-size: 30px;
}

.diana1 {
    color: red;
    font-size: 30px;
}

.diana2 {
    color: green;
    font-size: 30px;
}
</style>
