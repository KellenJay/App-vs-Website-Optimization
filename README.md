# App-vs-Website-Optimization

# StyleSync: A Data-Driven UX & Revenue Optimization Project

## Project Objective

This project was developed for *StyleSync*, a fictional online fashion retailer offering personalized in-store styling followed by online purchasing through a mobile app or desktop website. The business goal was to determine which platform—**mobile or web**—should be prioritized for user experience (UX) improvements in order to maximize customer lifetime value (CLV) and drive revenue.

This end-to-end case study centers on **Maya**, a fictional persona representing a real-world shopper who begins her journey with a 30 minute in-store style consultation and completes her purchase online via app or website. While it’s common for e-commerce platforms to include product carousels during checkout to increase cart size, this project explores a more nuanced use case: customers like Maya, who have already received personalized recommendations from a stylist.

For these high-intent users, reducing cognitive load and streamlining checkout proved more effective. Through predictive modeling, behavioral segmentation, and A/B testing, we simulate a real-world data product workflow to guide context-aware digital design and investment decisions in retail.

---

## Phase 1: Regression Analysis – Understanding Revenue Drivers

We began with an exploratory regression analysis to understand what behavioral metrics most influence yearly revenue:

* **Simple Linear Regression:**

  * Feature: `Length of Membership`
  * Result: Cross-validated R² = **0.655**
  * Insight: Longer-tenured customers generate significantly more revenue.

* **Multiple Linear Regression:**

  * Features: `Time on App`, `Time on Website`, `Avg. Session Length`, `Length of Membership`
  * Result: Cross-validated R² = **0.983**
  * Insight: `Time on App` is a far stronger predictor of revenue than `Time on Website`, suggesting that mobile users are more engaged and profitable.

These findings informed our next step: validating whether web experience optimization could still offer revenue lift, despite app superiority in engagement.

---

## Phase 2: CLV Benchmarking – Measuring Business Impact

Using the pre-A/B test dataset, we calculated Customer Lifetime Value (CLV):

* **Pre-Test CLV:**

  * Avg. Yearly Spend: \$499.31
  * Avg. Membership Duration: 3.5 months
  * Resulting CLV: **\$147.03**

Post-A/B test, treatment group behavior suggested increased revenue:

* **Post-Test CLV:**

  * Avg. Yearly Spend (treatment): \$554.22
  * Resulting CLV: **\$163.19**

This **\~11% lift in CLV** proved the potential of small UX tweaks to yield measurable gains.

---

## Phase 3: A/B Test – Simplifying the Checkout Flow

We hypothesized that removing the “Similar Items” carousel on the **website** would reduce distraction and improve conversion.

* **Statistical Significance:** Achieved at α = 0.05
* **Practical Significance:** Monthly lift of \$4.95 exceeds 5% MDE
* **Guardrail Metrics:** No negative impact on retention

This reinforced our model findings: **UX friction on web impacts revenue**, and optimizing checkout clarity benefits the business.

---

## Persona-Centric Insights: Maya the Buyer

We anchored our analysis around *Maya*, a busy professional who values efficient, curated shopping experiences. Her preferences reflected those of high-intent users who quickly convert if the experience is seamless.

Maya’s behavior helped validate our UX changes and informed our platform-specific recommendations.

---
## Key UX & Business Trade-Offs

- **Upselling vs. Efficiency**  
  Reducing friction boosts conversions for high-intent users, but may limit upsell potential.

- **Short-Term vs. Long-Term Engagement**  
  Faster checkouts drive immediate revenue, but can lower product discovery.

- **Simplicity vs. Experience Depth**  
  Clean design improves usability, but risks diminishing browsing richness.

- **Personalization vs. Operational Complexity**  
  Tailored UX improves outcomes, but adds design and maintenance overhead.

- **Confidence vs. Scalability Risk**  
  A/B test wins may not hold at scale without ongoing validation.

---

## Final Recommendation

Despite the mobile app’s stronger baseline performance, the A/B test revealed that **modest UX improvements to the website** still yield high returns. We recommend:

* **Rolling out the simplified checkout** experience for this user segment; those who received curated recommendations during in-store consultations.
* Continuing investment in mobile engagement based on regression findings
* Using CLV as a recurring metric for future UX evaluations

---

## Files in This Repository

* `Ecommerce Regression Model.ipynb` – Exploratory regression analysis
* `AB Test.ipynb` – Experimental design and treatment evaluation
* `README.md` – Project overview, results, and business implications

---

## Tools Used

* Python (pandas, sklearn, matplotlib, seaborn)
* Jupyter Notebooks
* Experimental Design & Statistical Testing
* Figma

---

## Author

**Ellen Ivanovic**
Product & Data Analyst 
