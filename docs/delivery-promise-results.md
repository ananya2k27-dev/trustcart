# Delivery promise experiment: results

Test set: 19286 delivered orders from 2018-05-26 to 2018-08-29 (model trained on 77141 earlier orders).

- Platform promise: average 21.99 days, **3.48% late**.
- At the SAME average length, the quantile model was late **1.73%** of the time; one fixed window for all orders was late 2.84%.
- To reach the platform's late rate, the quantile model needed an average promise of **18.33 days** (fixed window: 20.61 days) versus the platform's 21.99 days.
- 95% bootstrap interval, late-rate points saved at equal length: [1.57, 1.98]; days saved at equal late rate: [3.37, 4.04].
- Reviews: mean score 4.29 when on time vs 2.27 when late (n=95783).

## Caveats
- Olist is Brazilian marketplace data (2016-2018), not Indian.
- Only one chronological split; results can differ for other periods.
- Order-level features only; no carrier or route data.
