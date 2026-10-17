# Week 1 Data Engineering Lab

## Scenario
A small online shop sends daily order data as a CSV file. A manager wants a reliable summary of valid orders by city.

## Pipeline plan
- Source: `orders.csv` (daily batch file)
- Raw destination: BigQuery table `de_intro.raw_orders`
- Curated output: query results after checking and filtering the data
- User of the output: shop manager

## Local data check
Before reporting, record at least two issues you found in the CSV and what you recommend doing with each.
1. Issue and recommendation: Order O-1004 has a missing customer_city. Exclude it from the city report (or ask the shop to fix the source data).
2. Issue and recommendation: Order O-1005 has quantity 0. Exclude it because it is not a valid sale.
3. Issue and recommendation: Order O-1006 appears twice. Keep only one copy so it isn't counted twice.

## What the pipeline does
Complete after the lab: In one sentence, describe how the data moves from the source to a useful output.
