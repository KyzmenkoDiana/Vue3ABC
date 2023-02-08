<script>
import { enableTracking } from '@vue/reactivity';

export default {
    data() {
        return {
            diana: ['Vector', 'Flaffi', 'Djuliet', 'Diana', 'Polina'],

        }
    },
    methods: {
        Diana: function (index) {
            this.diana.splice(index, 1);
        }
    }
}
</script>

<template>
    <ul>
        <li class="diana" v-for="(item, index) in diana" :key="index">
            {{ item }}
            <button @click="Diana(index)">remove</button>
        </li>
    </ul>
</template>
<style>
.diana {
    color: blue;
}
</style>