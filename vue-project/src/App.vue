<script>
export default {
    data() {
        return {
            hrefs: [
                { href: '1.html', text: 'diana1' },
                { href: '2.html', text: 'diana2' },
                { href: '3.html', text: 'diana3' },
            ],
            products: [
                {
                    name: 'Djulia',
                    price: 100,
                    quantity: 5
                },
                {
                    name: 'Vector',
                    price: 200,
                    quantity: 4
                },
                {
                    name: 'Flaffi',
                    price: 300,
                    quantity: 3
                },
            ]
        }
    }
}
</script>

<template>
    <ul>
        <li v-for="link in hrefs"><a class="diana" hrefs="{{ link.href }}">{{ link.text }}</a></li>
    </ul>
    <b>
    </b>
    <table>
        <tr class="diana2" v-for="col in products">
            <td>{{ col.name }}</td>
            <td>{{ col.price }}</td>
            <td>{{ col.quantity }}</td>
        </tr>
    </table>
</template>
<style>
.diana {
    color: red;
    font-size: 20px;
}

.diana2 {
    color: blue;
    font-size: 20px;
}
</style>