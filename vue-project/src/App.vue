<script>
export default {
    data() {
        return {
            Dina: true,
            diana: true,
            style: {
                hidden: true,
            }
        }
    },
    methods: {
        setDone: function () {
            this.style.hidden = false;
        },
        setTwo: function () {
            this.style.hidden = true;
        },
        Diana: function () {
            this.Dina = !this.Dina;
        }
    }
}
</script>

<template>
    <button @click="Diana">Avocado</button>
    <p class="Avocado" v-if="Dina">Avocado</p>
    <p :class="style">Avocado</p>
    <button @click="setDone">показывает</button>
    <button @click="setTwo">прячет</button>

</template>


<style>
p {
    color: blue;
    font-size: 20px;
}

.Avocado {
    color: red;
    font-size: 20px;
}

p.hidden {
    display: none;
}
</style>