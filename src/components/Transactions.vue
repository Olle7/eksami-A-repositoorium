<template>

    <table>
      <p>{{sortedTransactions}}</p>
        <tr>
            <td>From / To</td>
            <td id="amount-label">Amount</td>
            <td>Currency</td>
        </tr>
      <tr v-for="transaction in transactions" :key="transaction.to">
        <td v-if="transaction.type === 'spending'" style="color: red">{{transaction.to}}</td>
        <td v-if="transaction.type === 'spending'" style="color: red">{{transaction.amount}}</td>
        <td v-if="transaction.type === 'spending'" style="color: red">{{transaction.currency}}</td>


        <td v-if="transaction.type === 'income'" style="color: green">{{transaction.from}}</td>
        <td v-if="transaction.type === 'income'" style="color: green">{{transaction.amount}}</td>
        <td v-if="transaction.type === 'income'" style="color: green">{{transaction.currency}}</td>
      </tr>


        <tr>
            <td colspan="3" style="text-align: right;">
                <span>Balance: <span id="balance"></span> EUR</span>
            </td>
        </tr>
    </table>
</template>

<script>
    export default {
        name: 'HelloWorld',
        props: {
            transactions: Array
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    table {
        width: 50%;
        margin: 0 auto;
    }
</style>