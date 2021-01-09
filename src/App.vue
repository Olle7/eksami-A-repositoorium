<template>
    <div id="app">
        <Transactions :transactions="transactions"/>
    </div>
</template>

<script>
    import Transactions from './components/Transactions.vue'

    export default {
        name: 'App',
        components: {
            Transactions
        },
        data: function () {
            return {
                transactions: [
                    {
                        to: "John Doe",
                        amount: 100,
                        currency: "EUR",
                        type: "spending"
                    },
                    {
                        from: "Unknown OU",
                        amount: 2045.87,
                        currency: "EUR",
                        type: "income"
                    },
                    {
                        to: "Jane Doe",
                        amount: 200,
                        currency: "EUR",
                        type: "spending"
                    },
                    {
                        to: "Generic Store",
                        amount: 10.7,
                        currency: "EUR",
                        type: "spending"
                    },
                    {
                        from: "Bob Smith",
                        amount: 50.7,
                        currency: "EUR",
                        type: "income"
                    },
                    {
                        from: "Grandma",
                        amount: 150,
                        currency: "EUR",
                        type: "income"
                    },
                    {
                        to: "Amazon",
                        amount: 76.90,
                        currency: "EUR",
                        type: "spending"
                    },
                    {
                        to: "Bolt",
                        amount: 4.5,
                        currency: "EUR",
                        type: "spending"
                    },
                    {
                        to: "Bill Newsome",
                        amount: 9.6,
                        currency: "EUR",
                        type: "spending"
                    },
                ]
            }
        }
    }
</script>

<style>
    #app {
        font-family: Avenir, Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }
</style>
