<script>
export default {
    data() {
        return {
            checked: true,
        }
    },
    methods: {
        toggle: function () {
            this.checked = false;
        }
    }
}
</script>

<template>
    <input class="diana" type="checkbox" v-model="checked">
    <p class="diana1" v-if="checked">{{ checked? 'Hello Diana': 'no' }}</p>
</template>
<style>
.diana {
    color: blue;
    font-size: 20px;
}

.diana1 {
    color: red;
    font-size: 20px;
}

.diana2 {
    color: green;
    font-size: 20px;
}
</style>