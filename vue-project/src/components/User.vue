<script>
export default {
    props: ['arg'],
    data() {
        return {
        }
    }
}
</script>

<template>
    <ul class="styled">
        <li class="diana" v-for="Avocado in arg">{{ Avocado }}</li>
    </ul>
</template>