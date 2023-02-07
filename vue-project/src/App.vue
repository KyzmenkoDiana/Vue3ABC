<script>
export default {
    data() {
        return {
            isAdmin: true,
        }
    }
}

</script>

<template>
    <p class="diana" v-if="isAdmin">+++</p>
    <p v-else>---</p>
</template>
<style>
.diana {
    color: blue;
    font-size: 30px;
}
</style>
