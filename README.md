# pcalc-functions #


A set of user-defined functions for [PCalc][1]. Email them to yourself, open the email on your iOS device, and you'll be able to import them into PCalc.

These functions were created with the help of the great PCalc function reference:  [All This : PCalc 2.8](https://leancrew.com/all-this/2013/05/pcalc-2-8/)


## Financial 2 ##

A simple set of functions for determining the time value of money:

### Future Value ###

A coefficient for calculating the future value of an investment. To get the future value, you multiply this number by the present value.

* Inputs
    + Y register: interest rate per compounding period
    + X register: number of compounding periods
* Output
    + X register: the future value coefficient


### Present Value ###

A coefficient for calculating the present value of an investment. To get the future value, you multiply this number by the future value.

* Inputs
    + Y register: interest rate per compounding period
    + X register: number of compounding periods
* Output
    + X register: the present value coefficient

### Loan Payment ###

A coefficient for calculating the periodic payment of a loan. To get the payment amount, you multiply the initial principal by this coefficient.

* Inputs
    + Y register: interest rate per period
    + X register: number of periods in the loan
* Output
    + X register: the payment coefficient

### Loan Interest ###

A coefficient for calculating the total interest of a loan. To get the interest amount, you multiply the initial principal by this coefficient.

* Inputs
    + Y register: interest rate per period
    + X register: number of periods in the loan
* Output
    + X register: the total interest coefficient


## Probability ##

A set of functions for probability distributions.

### Std Normal PDF ###

The probability density function of a standard normal variable.

* Input
    + X register: the value of the variable, x
* Output
    + X register: the value of the standard normal PDF at x

### Std Normal CDF ###

The cumulative density function of a standard normal variable.

* Input
    + X register: the value of the variable, x
* Output
    + X register: the value of the standard normal CDF at x


### Inverse Std Normal CDF ###

The inverse cumulative density function of a standard normal variable.

* Input
    + X register: the probability, p
* Output
    + X register: the value of the variable, x, associated with p


## Weather ##

Functions for determining the "feels like" temperature.

### Wind Chill ###

The wind chill index for cold and windy days.

* Inputs
    + Y register: the wind speed in mph
    + X register: the temperature in °F
* Output
    + X register: the wind chill index, a "feels like" temperature in °F

### Heat Index ###

The heat index for hot and humid days.

* Inputs
    + Y register: the relative humidity in %
    + X register: the temperature in °F
* Output
    + X register: the heat index, a "feels like" temperature in °F

## Change Log ##

* May 1, 2013
    + Initial Commit
* March 27, 2024
    + Added Loan Interest calculation

[1]: https://itunes.apple.com/us/app/pcalc-the-best-calculator/id284666222?mt=8&partnerId=30&siteID=L4JhWyGwYTM
