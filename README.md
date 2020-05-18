# Implement Multi Factor Model in OOP

From the Famma French Model, returns can be attributed to market factors. This notebook implements the model with market risk premium, plus 5 common factors premium. The script aims to make the model works and more reusable. Also, provides a rough picture of the factor performance. So there is nothing about model accuracy and parameters tunning here.

The data are queried from Quantopian and code is in python. The universe chosen is US top 1000 cap size stocks, feel free to edit in class "get_data". The class "factor_model" allows you to input fundamentals and pararmeters such as period of coverage, windows length, benchmark etc.

factor_model().a_r_prem will then return the factor risk premium.

Here are the factors I used:

Size: Market Cap, High minus Low

Value: P/B ratio, Low minus High

Quality: ROE - D/E, High minus Low

Momentum: Return on first 11 month of the last 12 month, High minus Low

Min Volatility: Annualized Volatility of daily return, Low minus High

Results: https://github.com/lauwo711/Multi-Factor-model/blob/master/Analysis.ipynb

Code: https://github.com/lauwo711/Multi-Factor-model/blob/master/Main.ipynb
