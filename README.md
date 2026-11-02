# Marketing Campaign Dashboard (Excel)

A four-page Excel dashboard that compares paid campaign performance across **Facebook, Instagram and Pinterest**, from March to November.

![Overview](images/overview.png)

## Business Question

Where should the marketing budget go? The dashboard answers three things:

1. How do impressions, engagement and conversions trend month by month?
2. Which channel, city, campaign season and device convert best?
3. Which channel returns the most conversion value per dollar spent?

## Key Results

| Metric | Total |
|---|---|
| Impressions | 14.65M |
| Likes | 608K |
| Shares | 119K |
| Conversion Value | $1.73M |
| Spend | $163K |
| **Overall ROAS** (Conversion Value ÷ Spend) | **10.6** |

### Channel Comparison

| Channel | Conversion Value | Spend | ROAS |
|---|---|---|---|
| Pinterest | $634.7K | $28.2K | **22.5** |
| Instagram | $684.8K | $63.4K | 10.8 |
| Facebook | $412.2K | $71.6K | 5.8 |

## Insights

- **Instagram is the top channel by conversion value** ($684.8K), but **Pinterest is the most efficient**: it returns about $22 for every $1 spent, roughly 4x Facebook.
- **Facebook has the highest spend and the lowest return.** It takes about 44% of the budget while producing about 24% of conversion value.
- **Performance steps up from September.** Monthly conversion value jumps from $157K in August to $236K in September and reaches $259K in November, the top month. Spend rises in the same period.
- **London leads impressions on all three channels**, while Manchester is the top city by conversions.
- Click-through rate trends upward on every platform from September onward.

## Recommendations

1. Shift part of the Facebook budget to Pinterest and test whether its ROAS holds as spend scales.
2. Keep Instagram as the volume channel, since it has the highest conversion value with a healthy ROAS.
3. Plan heavier campaigns for September to November, when conversion value is highest.

## Dashboard Pages

| Page | What it shows |
|---|---|
| **Marketing Campaign Dashboard** (Overview) | Combined KPIs, Spend vs Conversions, CTR per month, conversions and spend by channel and device, top month, top city and top channel |
| **Facebook Campaign Analysis** | Platform KPIs, Spend vs Conversions, CTR per month, Impressions by city, Conversions per campaign season (Desktop vs Mobile), Likes, Shares and Comments trend |
| **Instagram Campaign Analysis** | Same layout as Facebook |
| **Pinterest Campaign Analysis** | Same layout as Facebook |

![Facebook Campaign Analysis](images/facebook-campaign-analysis.png)
![Instagram Campaign Analysis](images/instagram-campaign-analysis.png)
![Pinterest Campaign Analysis](images/pinterest-campaign-analysis.png)

## Tools and Techniques

- **Power Query**: data cleaning and transformation
- **Power Pivot**: data model and relationships
- **DAX**: measures for the KPIs and ratios such as ROAS
- **Excel**: PivotTables and Pivot Charts, combo charts (columns plus line), shape-based navigation between pages
- **Design**: custom light, calm color palette, KPI cards with icons, one consistent layout across all pages, hidden gridlines and hidden calculation sheets

## Design Decisions

- **One layout for all channels**, so the pages can be compared quickly and the structure is easy to maintain.
- **No slicers.** The data covers March to November with partial months, and each platform has its own page, so a channel filter would be redundant. A fixed monthly view keeps the charts consistent.
- **Overview CTR** is shown as a combined score across the three platforms. Each platform page shows that platform's own CTR.

## Data

- **Period:** March to November (partial months)
- **Fields used:** Impressions, Likes, Shares, Comments, CTR, Conversion Value, Spend, Channel, City, Campaign season, Device

## How to Use

1. Download the Excel workbook from this repository.
2. Open it in Microsoft Excel (desktop recommended, because the data model uses Power Pivot).
3. Use the side menu to move between the Overview and the three channel pages.
