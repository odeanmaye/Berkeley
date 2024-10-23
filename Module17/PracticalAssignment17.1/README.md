
# Findings

![Marketing Campaign Analysis](img.png)

## Business Understanding of the Problem
The classification goal was to predict whether clients of a Portuguese banking institution would subscribe to a term deposit based on data from direct marketing campaigns. The target variable (`y`) is binary, representing a "yes" or "no" response.

## Clean and Organized Data
The dataset was cleaned by removing rows with null or "unknown" values. Irrelevant columns like `contact`, `day`, and `month` were dropped. The final dataset contained 12 integer variables and 4311 samples.

## Interpretation of Descriptive and Inferential Statistics
- **Duration**: The length of the call is the strongest predictor of whether a client subscribes, confirmed across both Logistic Regression and Random Forest models.
- **Housing loan status**, **campaign count**, and **personal loan status** were moderately important.
- **Balance**, **age**, and **pdays** were significant in Random Forest but had a smaller impact in Logistic Regression.
- Lower importance variables include **job**, **education**, and **marital status**, which were found to be less predictive.

## Clearly Stated Findings
- **Duration** of the call is the strongest predictor of a positive response. Statistical analysis confirms that the longer the call, the higher the likelihood of a client subscribing.
- Logistic Regression and Support Vector Machine models showed a **1.7% improvement** over the baseline when using only the `duration` variable.
- Including other features such as **housing loan status** and **campaign count** resulted in smaller improvements, with a maximum increase of **1.53%**.

## Actionable Items for a Non-Technical Audience
- **Key Insight**: Focus marketing efforts on increasing call durations, as this was the most significant predictor of success.
- **Secondary Factors**: Consider financial factors such as the client’s **balance** and **housing loan status**, though these are less impactful than call duration.
- **Variable Importance**: Variables like **job** and **marital status** were found to have a lower impact on whether a client subscribes, and marketing strategies should prioritize more relevant factors.

## Next Steps and Recommendations
1. **Optimize Call Durations**: Marketing teams should focus on strategies that can increase the length of client interactions to boost subscription rates.
2. **Refine Campaign Targeting**: Leverage predictive features such as **balance**, **age**, and **pdays** for targeting, but place a higher emphasis on improving the quality and length of client calls.
3. **Simplify Predictive Models**: Use the top 5 key variables identified to maintain strong predictive power while reducing complexity.
