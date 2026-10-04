# Understand the project before adding it to your CV

1. **Read the data:** `pd.read_excel` loads rows into a DataFrame, a table in Python. Identify what one row represents: one invoice item line, not a whole order.
2. **Inspect it:** `isna().sum()` counts missing values; `duplicated()` identifies repeated full rows. Explain why missing customer IDs do not mean we should discard sales.
3. **Filter it:** `.loc[...]` keeps rows matching a condition. Explain why cancelled invoices are excluded from positive purchases but included in signed transactions.
4. **Calculate value:** quantity × unit price. Explain why this is not profit and why a negative quantity reduces the signed total.
5. **Group it:** `groupby('Month').sum()` combines line values by month. Explain why December 2011 cannot be compared as a full month.
6. **Rank products:** the signed ranking accounts for negative lines and excludes an explicit list of fees/adjustments. Find the cancelled PAPER CRAFT order in the notebook.
7. **Count customers:** frequency uses `nunique()` invoice numbers. One invoice with ten products still counts as one purchase invoice.
8. **Check results:** assertions reconcile separately calculated totals. They check consistency, not whether the data captures all business activity.

## Your own practice

- Re-run the notebook yourself and check that outputs appear.
- Change the country chart from top eight to top five and explain what changed.
- Find the second-highest complete month using `monthly`.
- Explain the difference between positive purchase value and signed transaction value in two sentences.
- Pick one limitation and describe what extra data would help resolve it.

## A truthful project description, after you can explain and run it

“Analysed 541,909 retail transaction rows using Python and pandas; documented cleaning assumptions, compared purchase and signed transaction values, and visualised monthly trends, product performance and customer activity.”

Do not claim machine-learning modelling or independently written code. If asked, explain that AI assisted development and describe the work you ran, reviewed and changed yourself.
