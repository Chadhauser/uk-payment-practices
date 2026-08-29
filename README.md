# UK Payment Practices 2017–2026

Aggregate figures from **114,758 statutory payment practices reports** filed by
large UK companies between 2017 and 2026.

Every large UK company must report, twice a year, how long it takes to pay
suppliers and what proportion it pays late. The reports are public, but they sit
as tens of thousands of individual filings. This is the aggregate.

## Two findings, and they point in opposite directions

### 1. Payment has improved, steadily, on every measure

| Year | Reports | Median days to pay | Paid within 30 days | Paid over 60 days | Not paid on time |
|---|---|---|---|---|---|
| 2017 | 861 | 36 | 50% | 9% | 24% |
| 2018 | 13,419 | 35 | 55% | 8% | 26% |
| 2019 | 14,999 | 34 | 56% | 8% | 23% |
| 2020 | 13,789 | 34 | 56% | 8% | 23% |
| 2021 | 13,414 | 33 | 59% | 7% | 20% |
| 2022 | 13,068 | 33 | 60% | 7% | 20% |
| 2023 | 13,106 | 32 | 62% | 6% | 19% |
| 2024 | 13,212 | 32 | 64% | 5% | 17% |
| 2025 | 12,721 | 32 | 64% | 5% | 15% |
| 2026 | 6,165 | **31** | **64%** | **5%** | **15%** |

Median time to pay has fallen from 36 days to 31. The share of invoices paid
within 30 days has risen from 50% to 64%. The share not paid within agreed terms
has fallen from 24% to 15%.

**This runs against the common claim that late payment is worsening.** On the
statutory data, it has improved every year since reporting began.

### 2. But most companies still pay slower than their own stated terms

| | Days actual minus agreed terms |
|---|---|
| 10th percentile | −16 |
| Lower quartile | −4 |
| **Median** | **+10** |
| Upper quartile | +25 |
| 90th percentile | +39 |

**65.5% of companies pay slower than the terms they publish themselves.**

Median overshoot is 10 days. The slowest tenth run 39 days beyond their own
stated terms.

Based on 7,490 companies where both stated terms and actual performance are
reported.

## Distribution across all reports

| Measure | n | p10 | Q1 | Median | Q3 | p90 |
|---|---|---|---|---|---|---|
| Average days to pay | 105,237 | 15 | 24 | 33 | 46 | 58 |
| % invoices not paid on time | 105,354 | 2 | 8 | 20 | 39 | 62 |
| Standard payment terms (days) | 84,792 | 2 | 7 | 30 | 30 | 45 |

The spread matters as much as the middle. A quarter of reports show more than
39% of invoices paid outside agreed terms, and the worst tenth exceed 62%.

## Method

- Source: the statutory Payment Practices Reporting service at
  `check-payment-practices.service.gov.uk`, full bulk export
- 114,758 reports parsed, covering periods ending 2017 to 2026
- Reports are filed twice yearly by companies meeting the size thresholds under
  the Reporting on Payment Practices and Performance Regulations 2017
- Medians rather than means throughout, because a small number of extreme values
  would otherwise dominate
- Values outside plausible ranges excluded: days to pay under 0 or over 400,
  percentages outside 0–100
- Each measure reports its own sample count, because not every company completes
  every field
- Promise versus practice uses the most recent report per company, comparing
  average time to pay against the shortest stated standard payment period

## Limitations

**2026 is a partial year.** 6,165 reports against roughly 13,000 in a full year.
The figures look consistent with 2025 but should be treated as provisional.

**Only large companies report.** The thresholds capture companies above two of:
£36m turnover, £18m balance sheet total, 250 employees. Nothing here describes
how small companies pay.

**Self-reported.** These are the companies' own figures, filed under a statutory
duty but not independently audited.

**"Shortest standard payment period" is an imperfect comparator.** Companies with
several payment terms report a range; this uses the shortest, which is the most
generous reading. The true overshoot is likely larger than shown.

**No sector breakdown.** SIC codes are not part of the payment practices filing.
Company numbers are included in the source data, so a sector join is possible but
is not attempted here.

## Files

| File | Contents |
|---|---|
| `uk_payment_trend_by_year.csv` | Annual medians, 2017 to 2026 |
| `uk_payment_distribution.csv` | Quartiles and deciles across all reports |
| `uk_promise_vs_practice.csv` | Gap between stated terms and actual payment |

## Licence

CC BY 4.0. Free to use, including commercially, with attribution.

The underlying reports are public data published under the Open Government
Licence v3.0.

## Citation

> Edwards, P. (2026). *UK Payment Practices 2017–2026*. Finance Clearly.

## Corrections

If you find an error, please open an issue. Corrections are published with a
visible note rather than quietly fixed.

---

Compiled by Peter Edwards ACMA CGMA, a chartered management accountant, at
[Finance Clearly](https://financeclearly.com).
