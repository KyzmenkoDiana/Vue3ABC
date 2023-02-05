<script>
export default {
    data() {
        return {
            text: 'Diana',
        }
    },
    methods: {
        change: function () {
            this.text = 'Polina';
        },
        change2: function () {
            this.text = 'Diana';
        }/*тут и 1 и 2 и 3 задание*/
    }
}
</script>

<template>
    {{ text }}
    <button @click="change">text</button>
    <button @click="change2">text</button>
</template>

