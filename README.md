# European Option Pricing and Greeks Calculation Using QuantLib

## Description

This Python script demonstrates the process of pricing European call and put options using the Black-Scholes model, 
along with calculating the option Greeks (Delta, Gamma, Vega, Theta, Rho) for sensitivity analysis. 
The QuantLib library is utilized to model the financial instruments, set the market parameters, and perform the necessary calculations.

## Requirements
Python 3.x

QuantLib library

#### To install QuantLib, you can use pip:
pip install QuantLib

## Code Explanation
### 1. Market Parameters:

1. spot_price: Current stock price.
2. strike_price: Strike price of the option.
3. interest_rate: Annual risk-free rate.
4. volatility: Annual volatility of the asset.
5. time_to_maturity: Time until the option expires (in years).

### 2. Yield Curve and Volatility Structure:

The script defines the risk-free yield curve using a flat forward curve with the given interest rate.
The volatility structure is set using a constant volatility assumption.

### 3. Black-Scholes Process:

A Black-Scholes process is created with the spot price, risk-free rate, and volatility.

### 4. European Call and Put Options:

European call and put options are defined using the strike price and time to maturity.

### 5. Pricing Engine:

The options are priced using the AnalyticEuropeanEngine based on the Black-Scholes model.
### 6. Option Prices:

The script calculates and prints the prices of both the European call and put options.
### 7. Greeks Calculation:

The function print_greeks computes and prints the option Greeks for both call and put options: Delta, Gamma, Vega, Theta, and Rho.
