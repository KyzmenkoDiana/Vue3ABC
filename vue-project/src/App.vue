<script>
export default {
    data() {
        return {
            num1: 48,
            num2: 25,
        }
    },
    methods: {
        show: function (str) {
            return str[0].toUpperCase() + str.slice(1);
        }
    }
}
</script>
<template>
    <div>{{ num1 + num2 }}</div>
</template>

