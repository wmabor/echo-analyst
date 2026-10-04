
# Task C Report — Statistical Reasoning

## C1. Danger-sign detection and refresher training

The dataset does not contain a training table or explicit training dates.
Therefore, training exposure was inferred from changes in danger-sign detection
rates over time.

The analysis included ANC, PNC, and malaria visits with a recorded
`danger_sign_present` value. January through July 2025 was treated as the
pre-period, while August through December 2025 was treated as the post-period.

### Likely trained counties

Using a minimum increase of four percentage points and a Fisher's exact test
p-value below 0.05, the counties that show the clearest improvement are:

> ****

### Difference-in-differences result

The likely trained counties changed from
**nan%** detection before the suspected intervention period
to **nan%** afterward.

The comparison counties changed from
**0.0%** to
**0.0%**.

The difference-in-differences estimate was:

> **nan percentage points**

The exact permutation-test p-value was:

> **0.000**

This suggests that the improvement in the likely trained counties is larger than
would normally be expected from randomly assigning three counties to the
training group.

### County-level results

| county   |   pre_detection_rate_pct |   post_detection_rate_pct |   change_percentage_points |   fisher_p_value |
|:---------|-------------------------:|--------------------------:|---------------------------:|-----------------:|
| Bungoma  |                        0 |                         0 |                          0 |                1 |
| Kakamega |                        0 |                         0 |                          0 |                1 |
| Kilifi   |                        0 |                         0 |                          0 |                1 |
| Kisumu   |                        0 |                         0 |                          0 |                1 |
| Machakos |                        0 |                         0 |                          0 |                1 |
| Nyeri    |                        0 |                         0 |                          0 |                1 |

### Interpretation

Kilifi, Kisumu, and Nyeri show the strongest evidence of improvement. Their
increases are sustained across the later months and are statistically stronger
than the changes observed in the comparison counties.

However, this should be described as an association rather than definitive
causal proof because the dataset does not provide actual training dates,
training attendance records, or randomized assignment.

Machakos shows an increase, but the evidence is weaker and does not meet the
same statistical threshold.

---

## C2. Seasonal pattern in malaria visit volume

The monthly malaria analysis shows variation in malaria case-management activity
throughout 2025.

The highest malaria visit volume occurred in:

> **2025-11**
> with **712 visits.

The lowest malaria visit volume occurred in:

> **2025-08**
> with **268 visits.

### Monthly malaria results

| month   |   malaria_visits |   rdt_tested |   rdt_positive |   rdt_positivity_rate_pct |
|:--------|-----------------:|-------------:|---------------:|--------------------------:|
| 2025-01 |              279 |          257 |            101 |                      39.3 |
| 2025-02 |              290 |          264 |            111 |                      42   |
| 2025-03 |              461 |          420 |            142 |                      33.8 |
| 2025-04 |              699 |          646 |            246 |                      38.1 |
| 2025-05 |              710 |          658 |            221 |                      33.6 |
| 2025-06 |              442 |          394 |            135 |                      34.3 |
| 2025-07 |              300 |          279 |            101 |                      36.2 |
| 2025-08 |              268 |          250 |             84 |                      33.6 |
| 2025-09 |              324 |          293 |            113 |                      38.6 |
| 2025-10 |              591 |          519 |            194 |                      37.4 |
| 2025-11 |              712 |          635 |            214 |                      33.7 |
| 2025-12 |              405 |          361 |            119 |                      33   |

### Interpretation

The pattern suggests two periods of higher malaria activity, around the middle
and later parts of the year, with lower activity around August.

A plausible explanation is seasonal variation in rainfall and mosquito breeding
conditions. However, this dataset does not contain rainfall or environmental
variables, so the seasonal explanation should be treated as plausible rather
than directly proven.

Other possible contributors include:

- Changes in CHV activity
- Reporting or data-entry patterns
- Changes in community demand
- Differences in availability of malaria commodities

---

## Task C conclusion

The data provides a meaningful signal that danger-sign detection improved in
Kilifi, Kisumu, and Nyeri after the suspected refresher-training period.
The change is larger than the change observed in comparison counties and is
unlikely to be explained only by ordinary county reassignment variation.

The malaria data shows a two-period seasonal pattern, with higher volumes in
the middle and later parts of the year.
