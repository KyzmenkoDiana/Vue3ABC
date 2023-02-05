<script>
export default {
    data() {

    },
    methods: {
        show: function () {
            alert(new Date().toLocaleDateString());
        }
    }
}
</script>
<template>
    <!-- <button @click="show">По клику</button>-->
    <button v-on:mouseover="show">Мышкой</button>
</template>
