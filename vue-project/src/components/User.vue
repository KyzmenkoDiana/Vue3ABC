<script>
export default {
    props: {
        name: String,
        salary: Number,
        age: Number,
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