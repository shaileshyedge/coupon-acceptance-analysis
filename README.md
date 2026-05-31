# Will a Customer Accept the Coupon?

## Project Overview
This project explores survey data collected via Amazon Mechanical Turk to understand what factors influence whether a driver accepts a coupon delivered to their phone while driving. The dataset includes information about the driver, their passengers, the driving context, and the type of coupon offered.

## Key Question
**What characteristics distinguish drivers who accept coupons from those who do not?**

---

## Dataset
- **Source:** UCI Machine Learning Repository
- **Size:** 12,684 records, 26 features
- **Coupon Types:** Bar, Coffee House, Restaurant(<$20), Restaurant($20–$50), Carry Out & Take Away
- **Target Variable:** Y = 1 (accepted), Y = 0 (rejected)

---

## Overall Findings
The overall coupon acceptance rate across all types was **56.84%**, meaning more than half of drivers accepted a coupon when offered one. However, acceptance rates varied significantly by coupon type and driver characteristics.

---

## Bar Coupon Analysis
- The overall bar coupon acceptance rate was **41.00%**
- Drivers who visited bars **more than 3 times a month** accepted bar coupons at a rate of **76.88%**, compared to only **37.07%** for infrequent visitors
- Drivers without kid passengers, under the age of 30, and outside farming/fishing/forestry occupations showed notably higher acceptance rates

**Key Insight:** The strongest predictor of bar coupon acceptance is existing bar-going behavior. The coupon reinforces a habit rather than creating a new one.

---

## Restaurant($20–$50) Coupon Analysis
- The overall acceptance rate for upscale restaurant coupons was **44.10%** — one of the lowest among all coupon types
- Drivers traveling with a **partner** had the highest acceptance rate at **63.12%**
- Acceptance was highest at **10AM (61.61%)**, suggesting drivers plan ahead for a later meal
- Mid-range income drivers ($25,000–$37,499) showed the highest acceptance at **51.10%**

**Key Insight:** Unlike bar coupons, upscale dining coupons are driven by social context. Couples and drivers planning ahead are most likely to accept them.

---

## Recommendations
1. **Bar coupons** should be targeted at frequent bar-goers traveling without children — habit is the best predictor
2. **Upscale restaurant coupons** should be delivered to drivers traveling with a partner, ideally in the morning hours
3. **Income alone is not a reliable predictor** — mid-range income drivers respond better to upscale dining coupons than the highest earners

---

## Tools Used
- Python, Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook

## Files
- `assignment5_1_starter.ipynb` — Full analysis notebook
- `data/coupons.csv` — Dataset
