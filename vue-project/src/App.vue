<script>
export default {
    data() {
        return {
            arr: [],
        }
    }
}
</script>

<template>
    <div class="diana">
        <input class="diana1" type="checkbox" v-model="arr" value="English">
        <label>English</label>
        <br>
        <input class="diana1" type="checkbox" v-model="
        arr" value="Turkish">
        <label>Turkish</label>
        <br>
        <input class="diana1" type="checkbox" v-model="arr" value="Ukrainian">
        <label>Ukrainian</label>
        <ol>
            <ul v-for="elem in arr">{{ elem }}</ul>
        </ol>
    </div>
    <br>
</template>
<style>
.diana {
    color: blue;
    font-size: 20px;
}

.diana1 {
    color: red;
    font-size: 20px;
}
</style>