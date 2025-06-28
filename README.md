# Quinpoint-Capital-Investment-Management-Challenge

*Made for the Tech Academia “Investment-platform” challenge*

This folder gives you synthetic data so you can build and test an online wealth-management app.  
Nothing here is linked to real clients or money.

---

## What each file / folder is for

| Name | What’s inside |
|------|---------------|
| **instruments.csv** | A short list of the four securities clients have invested in:<br>• Microsoft (`I01`)<br>• S&P 500 ETF (`I02`)<br>• BT Group (`I03`)<br>• Barclays PLC (`I04`) |
| **clients.csv** | The high-net-worth customers (name, email, ID). |
| **advisors.csv** | Relationship managers who look after those clients. |
| **portfolio_assignments.csv** | Tells you who owns a given portfolio and their respective advisor. |
| **/portfolio_holdings/** | One CSV per portfolio (e.g. `P003.csv`).  Shows what each portfolio bought to start with: buy date, price, quantity, starting value.  Quantities never change in this exercise. |
| **/prices/** | Daily closing prices for 2024.  One CSV per instrument (e.g. `I01.csv`). |
| **README.md** | This guide. |

---

## How the numbers fit together

1. **Start value**  
   Look in `portfolio_holdings/P003.csv` → `initial_value` column.  
   That is what the holding was worth on the buy date.
   
2. **Initial Portfolio’s value**  
   Take the  Initial Purchase Value` from `/portfolio holdings/PXXX.csv` and multiply by `Inital Quanity Purchased`.   

3. **Today’s value**  
   Take the latest `close_price` from `/prices/` and multiply by `Inital Quanity Purchased`.

4. **Return (%)**  
   `(today_value – initial_value) ÷ initial_value`.

That’s it—no extra buys or sells to track.

## Quick notes

* One currency for everything—pretend it’s all in pounds or dollars, your choice.  
* All people and numbers are invented for learning only.  

Have fun!


