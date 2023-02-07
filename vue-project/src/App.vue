<script>
export default {
    data() {
        return {
            Avocado: true,
        }
    },
    methods: {
        Diana: function () {
            this.Avocado = false;
        }
    }
}
</script>

<template>
    <!--1-->
    <button @click="Diana">Diana</button>
    <p class="Avocado" v-show="Avocado">Djulia</p>
    <!--
        2 - v-show будет всегда отрисовываться и оставаться в DOM, a v-if выполняет настоящую условную отрисовку.
        3 - v-if если условие ложно на момент первоначальной отрисовки, v-show элемент всегда отрисовывается
        4 - директиву v-show нельзя использовать на элементе template и она не работает с v-else.-->
</template>
<style>
.Avocado {
    color: blue;
    font-size: 30px;
}
</style>
