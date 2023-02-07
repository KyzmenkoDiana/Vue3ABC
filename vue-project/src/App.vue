<script>
export default {
    data() {
        return {
            obj: {
                done: false,
                selected: true,
            }
        }
    }
}
</script>

<template>
    <p :class="obj">Avocado</p>
</template>
<style>
.done {
    color: red;
    font-size: 20px;
}

.selected {
    color: blue;
    font-size: 20px;
}
</style>