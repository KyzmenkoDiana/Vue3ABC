<script>
import Employee from './components/User.vue'

export default {
    components: {
        Employee
    }
}
</script>

<template>
    <Employee name="Diana" surn="Kuzmenko" age="19" />
</template>
<style>
.diana {
    color: blue;
    font-size: 20px;
}
</style>