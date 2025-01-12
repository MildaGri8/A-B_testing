## Fast Food Marketing campaign A/B Test


A fast-food chain plans to add a new item to its menu. However, they are still undecided between three possible marketing campaigns for promoting the new product. In order to determine which promotion has the greatest effect on sales, the new item is introduced at locations in several randomly selected markets. A different promotion is used at each location, and the weekly sales of the new item are recorded for the first four weeks.

[Fast Food Data Set](https://www.kaggle.com/datasets/chebotinaa/fast-food-marketing-campaign-ab-test)

### Goal
GOAL is to evaluate A/B testing results and decide which marketing strategy works the best.

### Target Metric
Sales for each **Promotion**.


### Summary
- **Promotion 2** showed worst results. Both, total sales and average sales were the lowest between 3 groups.
- **Promotion 3** had highest **Total** sales. However because of inequality of assigning **LocationID's** to **Promotions** (less **LocationID's** in **Promotion 1** compared to **Promotion 3**) average sales were highest in **Promotion 1**
- A/B test results showed significant difference of **Promotion 2** from other groups. It's Median is ~40 lower than **Promotion 1**, and ~ 24 lower than **Promotion3**.
- A/B test results showed no statistically significant diffrence between **Promotion 1** and **Promotion 3** groups. Although diffrence of ~14 could be significant for business decisions.

Recomendations for decision:
- Analyze **Promotions 1** and **Promotion 3** additionaly to see if there is any kind of similarities between **Promotion** themselves what may caused similar results.
- Analyze **Promotions 1** and **Promotion 3** from Market size, store location perspective to see if this may have causes similar results, or maybe different markets react better to different promotions.
- If there is no possibility for additional analysis - **Promotion 1** can be chosen for marketing strategy as having highest sales.


### Structure
food.ipynb: Jupyter Notebook for this project,

WA_Marketing-Campaign.csv: data set for this project,

README.md: Provides an overview and instructions for the projects.