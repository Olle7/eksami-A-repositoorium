<template>
    <table>
        <tr>
            <td>From / To</td>
            <td id="amount-label">Amount</td>
            <td>Currency</td>
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