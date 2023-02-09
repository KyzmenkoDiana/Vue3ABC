<script>
export default {
    props: ['name', 'salary', 'age'],
    data() {
        return {
        }
    }
}
</script>

<template>
    <ul>
        <p class="diana">
            {{ name }}
            {{ salary }}
            {{ age }}
        </p>
    </ul>
</template>