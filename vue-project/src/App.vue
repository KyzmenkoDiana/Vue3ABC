<script>
export default {
    data() {
        return {
            language: '',
            d: false,
            di: false,
            diana: false
        }
    },
    methods: {
        Djuliet() {
            this.d = true;
        },
        Vector() {
            this.di = true;
        },
        Flaffi() {
            this.diana = true;
        }
    }
}
</script>

<template>
    <input type="radio" v-model="language" value="Turkish" @click="Djuliet">
    <p class="diana">Turkish</p>
    <p></p>
    <input type="radio" v-model="language" value="Ukrainian" @click="Vector">
    <p class="diana">Ukrainian</p>
    <p></p>
    <input type="radio" v-model="language" value="Russian" @click="Flaffi">
    <p></p>
    <p class="diana">Russian</p>
    <p class="diana1" v-if="d">Mahraba, benim adim Diana</p>
    <p class="diana1" v-else-if="di">Привiт, мене звуть Дiана</p>
    <p class="diana1" v-else-if="diana">Привет, меня зовут Диана</p>

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