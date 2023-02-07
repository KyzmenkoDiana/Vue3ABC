<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<template>
    <ul :class="{ active: true, valid: false }">
        Hello my name Diana
    </ul>
</template>
<style>
.active {
    color: blue;
    font-size: 20px;
}

.valid {
    color: red;
    font-size: 20px;
}
</style>