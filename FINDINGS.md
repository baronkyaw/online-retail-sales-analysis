# Findings and interpretation

- Source: 541,909 rows; positive purchase view: 524,878 rows after the documented cleaning steps.
- Positive purchase value: **£10,642,110.80**. Signed transaction value: **£9,748,131.07**. Negative recorded value: **£-893,979.73**. These are recorded transaction measures, not profit.
- **2011-11** had the highest signed value among complete observed months: **£1,456,145.80**. December 2011 is partial and excluded from this comparison.
- The UK contributes **84.0%** of signed transaction value. The dataset therefore mainly reflects this retailer's UK activity.
- Top merchandise code by signed value: **22423**, REGENCY CAKESTAND 3 TIER: **£164,459.49**.
- A £168,469.60 PAPER CRAFT order was cancelled 12 minutes later. It contributes zero signed value, illustrating why positive purchases alone can mislead product rankings.
- **4,338** known customer IDs; **65.6%** placed at least two distinct positive purchase invoices during this window.
- **16.5%** of positive purchase value has no customer ID; customer conclusions exclude those purchases.
- The rounded-up top 10% of known customers account for **61.5%** of known-customer positive purchase value. Check cancellations before treating this as evidence of customer value.
- Removing exact duplicate rows reduced positive purchase value by **£24,573.74**. This assumption is reproducible but cannot be proved from a unique line identifier.

All findings come from the included executed notebook and original UCI data. No sales forecast, causal claim, profit estimate or machine-learning accuracy is claimed.
