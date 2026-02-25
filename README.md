# Insurance Marketing Campaign Analysis

## Overview
This project analyzes customer responses to insurance marketing campaigns. The goal was to identify drivers of responsiveness, segment customers, and provide actionable recommendations for improving marketing effectiveness. The dataset contained ~9,000 customers with demographic, financial, policy, and campaign response information.

---

## Methodology
1. **Data Exploration**
   - Inspected dataset structure (24 columns, no missing values).
   - Target variable: `Response` (Yes/No).
   - Identified categorical vs. numerical features.

2. **Preprocessing**
   - Dropped irrelevant columns (`Customer`, `Effective To Date`).
   - Encoded categorical features.
   - Scaled numerical features for clustering/modeling.
   - Kept a copy (`df_viz`) for human‑readable plots.

3. **Exploratory Data Analysis (EDA)**
   - Majority of customers responded “No” (~82%), minority “Yes” (~18%).
   - Response rates varied across demographics, education, and policy details.
   - Correlation heatmap showed financial/policy variables strongly related to response.

4. **Customer Segmentation (KMeans)**
   - Clustered customers into 4 groups using financial/policy features.
   - Cluster 2 (higher income + higher claims) had the highest response rate (~17%).

5. **Response Rate Analysis**
   - Quantified response rates across all major drivers:
     - Renew Offer Type
     - Employment Status
     - Education
     - Income Bands
     - Customer Lifetime Value (CLV)
     - Monthly Premium Auto
     - Policy Inception
     - Sales Channel
     - Policy Type
     - Vehicle Size
     - Coverage
     - Location Code / State
     - Number of Policies
     - Months Since Last Claim

---

## Key Findings (Quantified)
- **Renew Offer Type**: Offer2 had the highest success (23% Yes), Offer1 at 15.8%, Offer3 at 2.1%, Offer4 at 0%.
- **Employment Status**: Retired customers responded at 72% Yes vs Employed at 13% (+59% lift).
- **Education**: Doctorates (17.5%) and Masters (16.2%) responded more than High School (13%).
- **Income Bands**: Low income customers were most responsive (24.6%), higher bands ~12–14%.
- **CLV Bands**: Medium/Very High CLV ~15% Yes, High CLV lower (~12%).
- **Monthly Premium Auto**: Certain premium levels (66, 76) showed spikes (~25–27% Yes).
- **Policy Inception**: Months 3–4 showed spikes (~20–26% Yes).
- **Sales Channel**: Agent channel converted best (19%), Call Center worst (11%).
- **Policy Type**: Special Auto highest (16.4%), Personal/Corporate ~14%.
- **Vehicle Size**: Large vehicles responded more (17.8%) than small (11.2%).
- **Coverage**: Premium slightly higher (14.6%) than Basic/Extended (~14%).
- **Location Code**: Suburban customers most responsive (17.4%), Rural/Urban ~9%.
- **State**: All ~14%, no major differences.
- **Number of Policies**: Customers with 9 policies responded 17.3%, others ~10–15%.
- **Months Since Last Claim**: Month 3 (22%), Month 10 (19.6%), Month 1 (19.1%) higher; Month 0 lowest (7.6%).

---

## Recommendations
1. **Optimize Renewal Offers**
   - Focus on Offer2 (+7.6% lift vs Offer1).
   - Discontinue or redesign Offer4 (0% success).

2. **Target Retired Customers**
   - Extremely receptive segment (72% Yes).
   - Tailor messaging and offers specifically for retirees.

3. **Leverage Income & CLV Segments**
   - Low income customers surprisingly most responsive (25% Yes).
   - Medium/Very High CLV also stronger (~15% Yes).
   - Campaigns should not ignore lower‑income groups.

4. **Channel Strategy**
   - Agent channel converts best (19% vs 11% Call Center).
   - Prioritize agent‑led campaigns for higher conversion.

5. **Policy & Vehicle Segments**
   - Special Auto policies (16.4%) outperform others.
   - Large vehicle owners (17.8%) more responsive than small (11.2%).

6. **Timing Campaigns**
   - Target customers at 3–4 months policy inception (20–26% Yes).
   - Focus on premium levels 66 and 76 (~25–27% Yes).

7. **Geographic Focus**
   - Suburban customers most responsive (17.4% vs 9% Rural/Urban).
   - Campaigns should emphasize suburban areas.

8. **Claims History**
   - Avoid targeting immediately after claims (7.6% Yes).
   - Focus on customers 3–10 months post‑claim (~20–22% Yes).

---

## Business Impact
- **Conversion Lift**: Targeting Offer2, retirees, suburban customers, and agent channels could increase conversions by 8–15 percentage points.
- **ROI Improvement**: Redirecting spend away from Offer4, unemployed customers, and urban/rural areas reduces wasted budget.
- **Strategic Segmentation**: Campaigns tailored by timing (policy inception, claims history) and product (vehicle size, policy type) maximize responsiveness.
- **Data‑Driven Decisions**: Quantified findings provide clear levers for marketing strategy, ensuring evidence‑based campaigns.

---

## Conclusion
This analysis provides a complete evidence‑based view of customer responsiveness. By focusing on the strongest drivers (Offer2, retirees, suburban customers, agent channels, timing at 3–4 months inception, certain premium levels), insurers can significantly improve campaign effectiveness and ROI.
