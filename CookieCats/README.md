## Cookie Cats A/B Test project


Cookie Cats is popular "connect- three" style puzzle game. When users progress through the game, they encounter "Gate" that forces users to wait some time, or to make In-app purchase to progress further. 

Having this in mind - the placement of the "Gate" has huge impact. Initially gate was placet at level 30. Experiment was conducted to see the impact of gate being moved to level 40. 

[Cookie Cats Data Set](https://www.kaggle.com/datasets/mursideyarkin/mobile-games-ab-testing-cookie-cats)


### Goal
Goal of A/B test is to compare 2 versions of the game (control - gate at level 30, experiment - gate at level 40) and determine which version performs better based on chosen metrics.

### Target metric
**Primary metric - Engagement**
- Compare average number of game rounds played between 2 groups to assess engagement. 

**Secondary metric - Retention**
- Retention on Day 1 (retention_1): Measure the proportion of players (%) who return on the first day after installation for both groups. This helps assess the immediate impact on retention.
- Retention on Day 7 (retention_7): Measure the proportion of players (%) who return on the seventh day after installation. This captures medium-term retention and whether players are more likely to stay engaged long enough to reach the gate.

### Summary
1. Desing of experiment should be addressed.
    - Eventhoug assigment to experiment and control groups can be treated as independent, sample ratio proportions were not kept. This becomes even more important after data clean up.
    - Additional information about experiment would be needed, like average number of gamerounds user plays to pass one level to make estimations more precise.
2. Results of analysis
    - Hypothesis tests showed significant differences between experiment and control groups for all target metrics.
    - Average number of **Gamerounds** users played after Gate is ~10 Gamerounds higher for experiment group. This suggests that moving gates makes users play more **Gamerounds**. More **Gamerounds** means that users spend more time playing, and could be potentially exposed to more adds.
    - Retention after 1 day is better by ~2.8%, after 7 days better by ~4.7% for experiment group compare to control group.
    - Gate movement not only makes users play longer, but also more users continue playing this game afer 1 and 7 days.


**Evaluating results from this analysis - it is recomended to implement gate change from level 30 to level 40.**


### Structure

cats.ipynb: Jupyter Notebook for this project.

cookie_cats.csv: data set for this project,

README.md: Provides an overview and instructions for this project.