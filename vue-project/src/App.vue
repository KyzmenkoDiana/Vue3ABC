<script>
export default {
    data() {
        return {

        }
    },
    methods: {
        show: function () {
            alert('!');
        }
    }
}

</script>

<template>
    <a class="inline-link-1" href="https://www.google.ru " onclick="event.preventDefault()">Diana</a>
    <br>
    <br>
    <button @click.once="show">Diana</button>
</template>

