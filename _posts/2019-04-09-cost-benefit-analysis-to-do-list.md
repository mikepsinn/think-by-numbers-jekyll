## Prioritize Your To-Do List By Converting Costs and Benefits To Present Value

There is an infinite number of ways you can spend your most valuable resource, time. How can you decide what the most cost-effective way to spend your time is? By converting the returns of each activity to its present value and picking the activity with the highest present value.

I live in a house that's bigger than I need and farther away from my job than I'd like. So I'd like to sell it and get a smaller apartment closer to work.

### Benefits of Moving

#### 1. Time Savings

It's also going to take a lot of time. In order to do apples to apples comparisons, we need to convert this time to a monetary value. According to the Bureau of Labor Statistics, the average American worker makes [$27/hour](https://www.bls.gov/news.release/empsit.t19.htm).

Moving closer to my job will save me 2 hours per week (an equivalent of $54 in weekly earnings). I assume I'll be working there for 4 more years. This gives us a total savings of $11,232 (52 weeks * $54/week * 4 years).

However, this is complicated by the fact that due to inflation and interest-earning potential, a dollar today is worth more than a dollar tomorrow. So to achieve an apples to apples comparison, we'll need to convert these savings to the equivalent Present Value.

 So let's calculate the equivalent present value of this expense. You can do this in Google Sheets with the following formula.

` Present Value = future_value/(1 + rate)^number_of_periods `

or in Google Sheets, you can use the formula:

` PV(rate, number_of_periods, future_value) `

- rate - This is the rate that you could get by investing this money.  [10%](https://www.nerdwallet.com/blog/investing/average-stock-market-return/) is the average annual rate of return for the stock market, so let's use that.
- number_of_periods - We're using the annual return and I'll be saving this drive for 4 years. So the number of periods is 4.
- future_value - We'll save $11k (52 weeks * $54/week * 4 years).

The result is a Present Value of $8k for the time savings from not having to drive so much.

#### 2. Rent Savings

Say my monthly mortgage payment is $1400/month.  I can get a smaller apartment for $900/month.  So I'll save $500 per month on rent.  After 4 years, that will save me $24k. Plugging those numbers into our PV formula gives us $15k.

####  3. Investment Income

Let's say you can sell your house for $200k.  We're going to need to subtract some costs from that.

#### Selling & Moving Expenses
Moving comes with a great cost. Assuming a sale price of $200,000, the typical costs of selling a house and moving are $33,330.

<iframe class="airtable-embed" src="https://airtable.com/embed/shrKWs8DhDmaQi6zn?backgroundColor=yellow&viewControls=on" frameborder="0" onmousewheel="" width="100%" height="533" style="background: transparent; border: 1px solid #ccc;"></iframe>

Also, assume you have $116k remaining on the principal of your mortgage. That brings our total proceeds down to $50k.
So far, our total PV we get from moving is $58k ($8 plus $50k).

### Future Costs

However, we need to consider the opportunity cost to sell our house in 20 years once the mortgage is paid off. The U.S. House Price Index shows that prices have risen at 3.4% per year on average since 1991, so we'll use that to illustrate our calculations.

To calculate the expected future value based on your growth rate, add one to the rate, and raise this to a power equal to the number of years you're looking at.

` future_value = (1 + annual_growth_rate) ^ years * current_value `

or

` (1 + 0.0034) ^ 20 years * $200k = $390k Future Value `

So in 20 years, our home should be worth $390k.  Let's convert that back to the Present Value so we can compare apples to apples.

` Present Value = $390k/(1 + 0.1)^(20 years) = $58k`

So in the long run, our benefits of moving are $58k - $58k opportunity cost = $0.


https://github.com/mikepsinn/think-by-numbers-jekyll/blob/master/wp-content/uploads/present-value-formula.gif?raw=true

