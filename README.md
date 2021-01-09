# wad20-exam2-a

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```


# Tasks

Modify [Transactions.vue](./src/components/Transactions.vue)
 so that it displays all the transaction objects that are passed to it from [App.vue](./src/App.vue)

1. Display From/To, amount and currency of each transaction _**[5 points]**_
2. Have a **computed property** called `sortedTransactions` 
that sorts received list by amount (largest to smallest by default) _**[6 points]**_
3. Have a **computed property** called `balance` that calculates 
total (adds amount of a transaction if `type` is `income`, 
subtracts if `type` is `spending`) and display it in the `span`
 element that has the **id** `balance` _**[6 points]**_
4. On click on the Amount label (element with id `amount-label`) 
toggle order of the list by amounts, from largest to smallest and vice versa _**[5 points]**_
5. Color the text in the row of a transaction to green if 
transaction `type` is `income` and red if it is `spending` _**[3 points]**_

Your app should look something like this:
![screenshot](./src/assets/screenshot.gif)

