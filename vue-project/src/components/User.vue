<script>
export default {
    props: ['name', 'surn', 'age'],
    data() {
        return {

        }
    }
}
</script>
<template>
    <p class="diana">{{ name }}</p>
    <p class="diana">{{ surn }}</p>
    <p class="diana">{{ age }}</p>
</template>