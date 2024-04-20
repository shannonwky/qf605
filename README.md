# QF605

## Part I (Bootstrapping Swap Curves)
1. In the IR Data.xlsm spreadsheeet, OIS data is provided. Bootstrap the OIS discount factor Do(0, T ) and plot the discount curve for T ∈ [0, 30].
2. Using the IRS data provided, bootstrap the LIBOR discount factor D(0, T ), and plot it for T ∈ [0, 30].
⇒ Assume that the swap market is collateralized in cash and overnight interest is paid on collateral posted.
3.Calculate the following forward swap rates:
• 1y × 1y, 1y × 2y, 1y × 3y, 1y × 5y, 1y × 10y
• 5y × 1y, 5y × 2y, 5y × 3y, 5y × 5y, 5y × 10y
• 10y × 1y, 10y × 2y, 10y × 3y, 10y × 5y, 10y × 10y
Use linear interpolation on discount factors when necessary.

## Part II (Swaption Calibration)
Under the Swaption tab of IR Data.xlsm, swaption implied volatilities (lognormal) are provided.
1. Calibrate the displaced-diffusion model to the swaption market data, and document
• a table of σ parameters
• a table of β parameters
2. Calibrate the SABR model to the swaption market data using β = 0.9, and document
• a table of α parameters
• a table of ρ parameters
• a table of ν parameters
3. Price the following swaptions using the calibrated displaced-diffusion and SABR model:
• payer 2y × 10y K = 1%, 2%, 3%, 4%, 5%, 6%, 7%, 8%
• receiver 8y × 10y K = 1%, 2%, 3%, 4%, 5%, 6%, 7%, 8%

## Part III (Convexity Correction)
1. Using the SABR model calibrated in the previous question, value the following constant maturity swap (CMS) products:
• PV of a leg receiving CMS10y semi-annually over the next 5 years
• PV of a leg receiving CMS2y quarterly over the next 10 years
2. Compare the forward swap rates with the CMS rate:
• 1y × 1y, 1y × 2y, 1y × 3y, 1y × 5y, 1y × 10y
• 5y × 1y, 5y × 2y, 5y × 3y, 5y × 5y, 5y × 10y
• 10y × 1y, 10y × 2y, 10y × 3y, 10y × 5y, 10y × 10y
Discuss the effect of maturity and tenor on convexity correction (difference between forward swap rates and CMS rates).

## Part IV (Decompounded Options)
1. A decompounded option pays the following at time T = 5y:
  CMS 10y ^ (1/p) − 0.04 ^ (1/q)
where p = 4 and q = 2. Use static replication to value the PV of this payoff.
2 Supose the payoff is now
[CMS 10y ^ (1/p) − 0.04 ^ (1/q)]+
Use static replication to value the PV of this payoff.
