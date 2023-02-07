<script>
export default {
    data() {
        return {
            cssClasses: 'Avocado',
        }
    }
}
</script>

<template>
    <p :class="cssClasses">Avocado</p>
</template>
<style>
.Avocado {
    color: red;
    font-size: 20px;
}

p1 {
    color: blue;
    font-size: 20px;
}
</style>