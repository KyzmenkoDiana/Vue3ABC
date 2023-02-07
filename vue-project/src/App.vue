<script>
export default {
    data() {
        return {
            isValid: true,
            isDisabled: true,
        }
    }
}
</script>

<template>
    <p :class="{ Valid: isValid }">
        Hello my name Diana </p>
    <b></b>
    <p :class="{ Disabled: isDisabled }">
        I life in Armyansk </p>
</template>
<style>
.Valid {
    color: blue;
    font-size: 20px;
}

.Disabled {
    color: red;
    font-size: 20px;
}
</style>