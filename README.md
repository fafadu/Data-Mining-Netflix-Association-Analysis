# Data-Mining-Netflix-Association-Analysis
The project aims to provide valuable insights into Netflix's content. 
Apriori Algorithm: Used for association analysis to uncover frequent itemsets among movie release countries.

### Data Source: https://www.kaggle.com/datasets/shivamb/netflix-shows

### Tools & Techniques: Python (Pandas, NumPy, Matplotlib, mlxtend), Apriori Algorithm, Association Rule Mining, Jupyter Notebook.

### Evaluation Metrics:
Lift: Measures the strength of associations between countries in terms of movie releases.
Parameter Settings:
Min Support (min_support): Set to 0.0065, meaning only itemsets that appear in at least 0.65% of the rows are considered frequent. This filters out low-frequency or rare itemsets.
Min Confidence Threshold (min_threshold): Set to 0.05, filtering out association rules with low confidence.

### Conclusion:
US Dominates Content: A large number of movies on Netflix are released in the United States, showing it as a key movie market.
Multi-Country Releases: Some movies are released in multiple countries simultaneously, such as "United States and United Kingdom" or "United States and Canada," reflecting Netflix's strong global presence.
Strong US-UK Connection: The United States and United Kingdom often appear together in release combinations, indicating collaboration or similar audience preferences in these two countries.
Most Rules Have Limited Impact: While some interesting association rules were found, most have low support and confidence, meaning they may be coincidental rather than strong patterns.

### Output and explination:
![output_2_1](https://github.com/user-attachments/assets/94ba4406-dd75-48dc-ac40-fb08de3a2501)
I set the min_support to 0.0065, which means that only itemsets that appear in at least 0.65% of the rows are considered frequent. This helps filter out low-frequency or rare itemsets. At the same time, I set the min_threshold to 0.05, filtering out association rules with low confidence. The country with the highest support value is "United States," which indicates that a significant number of movies on Netflix are released in the United States. Some frequent itemsets involve multiple countries, such as "United Kingdom, United States" and "Canada, United States." This suggests that there are movies frequently released in multiple countries, indicating Netflix's international presence. "United Kingdom" and "United States" frequently appear together in the same itemset, indicating that there might be regional preferences or collaborations in movie releases between these two countries.

![output_4](https://github.com/user-attachments/assets/9636a795-d78d-4038-a02d-8ccf98ba10ab)

 This table displays the association rules sorted by confidence in descending order. It includes columns for antecedents, consequents, antecedent support, consequent support, support, confidence, lift, leverage, conviction, and Zhang's metric for each rule. The rule (Belgium)-> (France) has a confidence of 0.6333, indicating that if a movie is available in Belgium, there's a strong likelihood it will also be available in France.

![output_3_0](https://github.com/user-attachments/assets/c1a34d7b-9a54-4cc8-9e85-2e34aea80940)
This Support and Confidence Scatter Plot visualizes the relationship between the support and confidence of association rules. The majority of rules are clustered in the lower-left quadrant, indicating that most rules have low support and low confidence and the points in the upper and right areas of the plot mean fewer rules have high support or high confidence, This information can be valuable for Netflix in terms of content distribution strategies. They can identify which countries or regions to focus on for certain types of content, potentially leading to better content recommendations for users in those areas.


專案目標：旨在提供關於 Netflix 內容的寶貴洞見。
Apriori 演算法：用於關聯分析，揭示電影發行國之間的頻繁項集。
工具與技術: Python（Pandas, NumPy, Matplotlib, mlxtend）, Apriori Algorithm, Association Rule Mining, Jupyter Notebook
評估指標：
提升度 (Lift)：用於評估國家之間在電影發行方面的關聯性，表明關聯的強度。
參數設置
最小支持度 (min_support)：設定為 0.0065，這表示僅考慮在至少 0.65% 的資料列中出現的項集，從而過濾掉低頻或稀有的項集。
最小置信度閾值 (min_threshold)：設定為 0.05，過濾掉置信度較低的關聯規則。
結論:
美國主導內容：Netflix 上有大量電影是在美國發行的，這顯示美國是主要的電影市場。
多國同步發行：有些電影會同時在多個國家發行，比如「美國和英國」或「美國和加拿大」。這表明 Netflix 在全球有很強的國際布局。
英國和美國的緊密關聯：英國和美國經常一起出現在電影發行的組合中，可能反映這兩國在電影市場上的合作或觀眾喜好相似。
大部分關聯規則影響力有限：雖然發現了一些有趣的關聯規則，但多數規則的影響力（支持度和置信度）都不高，可能只是偶然關聯。
