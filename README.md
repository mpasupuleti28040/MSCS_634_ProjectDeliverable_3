# MSCS_634_ProjectDeliverable_3
# Mall Customer Segmentation and Pattern Mining

## Project Overview
In this project, I applied classification, clustering, and association rule mining techniques to the **Mall Customers Dataset** to gain insights into customer behavior. The dataset includes customer demographics such as gender, age, annual income, and spending score. Using machine learning models, I aimed to develop predictive models, identify customer segments, and uncover meaningful patterns that can be applied in real-world scenarios.

## Key Insights
* **Classification Models**: 
  * The **Decision Tree** model performed excellently, achieving perfect accuracy and F1 score, making it highly effective for predicting customer gender based on demographic features.
  * The **k-Nearest Neighbors (k-NN)** model, although optimized through hyperparameter tuning, showed lower performance compared to the Decision Tree. Its accuracy was around 51%, indicating that further improvements could be made.

* **Clustering**:
  * I applied **K-Means clustering** to segment customers based on age, annual income, and spending score. The clustering results identified several customer groups, such as younger, low-income individuals with high spending scores, and older, higher-income customers with moderate spending scores. This segmentation can be useful for targeting specific marketing campaigns.

* **Association Rule Mining**:
  * Using the **Apriori** algorithm, I uncovered associations between customer demographics and spending behavior. For example, younger customers with lower incomes were more likely to have lower spending scores, while older customers with higher incomes tended to have higher spending scores. These rules can help businesses design better product recommendations and marketing strategies.

## Practical Relevance
The insights from this project can be applied in various real-world business contexts:
* **Targeted Marketing**: By identifying customer segments through clustering and association rules, businesses can tailor their marketing efforts to different groups, increasing the effectiveness of their campaigns.
* **Customer Profiling**: The classification models can help businesses predict customer characteristics based on demographic data, enabling better customer profiling and service personalization.
* **Product Recommendations**: The association rules can be used to identify products that are frequently purchased together, leading to more accurate product recommendations and promotions.

## Challenges Encountered
* **Imbalanced Data**: The k-NN model faced challenges due to the imbalanced distribution of genders in the dataset. I addressed this by performing hyperparameter tuning to find the best number of neighbors, but further improvements could be made by exploring other techniques like resampling or using different classifiers.
   
* **Binning Continuous Data for Association Rules**: For association rule mining, I had to bin continuous variables (age, income, and spending score) into categories. This process was tricky, as I had to balance between preserving the information and creating useful categorical groups. Ultimately, I chose a simple binning approach, but it’s important to consider that more complex binning strategies could yield different results.

* **Interpretability of Clustering**: While K-Means successfully grouped customers into distinct clusters, interpreting and labeling these clusters required domain knowledge. Understanding the true business value of each cluster can be subjective, but the clustering did provide a solid starting point for customer segmentation.

## Conclusion
This project demonstrated the application of machine learning techniques to understand customer behavior and gain insights into their demographics and spending patterns. The classification models, clustering, and association rule mining all provided valuable findings that can be directly applied to improve business strategies, such as marketing, customer segmentation, and product recommendations. Despite a few challenges in data preparation and model optimization, the project successfully identified key patterns and provided actionable insights that can guide real-world decision-making.
