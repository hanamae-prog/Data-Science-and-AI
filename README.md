# DATA VISUALIZATION: MALNUTRITION
Submitted by: 
Anonuevo, John Carlo S.

Bautista, Jericho 

Carreon, Hannah Mae B.

Librea, Mark Gelo M.

Torres, Tyrone Bruce

![image](https://github.com/hanamae-prog/Data-Science-and-AI/assets/137803175/bd846148-6c2b-4416-bd27-bd152aec0808)




Submitted to: Engr. Aisa M. Labastilla 

Date: January 23, 2023

# INTRODUCTION
Malnutrition is one of the prominent social issues across the globe. It is a condition that results from an inadequate or unbalanced diet, which has a significant social implication. Moreover, it can affect individuals, families, and communities, and it is often associated with broader socio-economic factors. It encompasses three primary categories of conditions: undernutrition, comprising wasting, stunting, and underweight; micronutrient-related malnutrition; and overweight, obesity, and diet-related issues. Malnutrition is a pervasive global issue, impacting individuals universally. In 2014, 462 million adults were underweight, and 1.9 billion were overweight or obese globally. Approximately 155 million children under 5 years experienced stunting, with 41 million being overweight or obese. Undernutrition is associated with 45% of deaths in children under 5 years old [1].

Moreover, the goal of this project is to predict malnutrition levels, encompassing severe wasting, wasting, overweight, stunting, and underweight through a comprehensive approach. Initial steps involve meticulous data preparation, including cleaning and preprocessing. Logistic regression is employed for binary classifications, with the dataset split into training and testing sets. For multi-class scenarios, decision trees and random forests are explored. Deep learning models using TensorFlow Keras capture intricate patterns. Performance metrics guide model evaluation and hyperparameter tuning optimizes parameters. Models are validated on new data for generalization, offering insights into malnutrition factors. The iterative process ensures continuous improvement based on feedback and new data, striving for a robust and accurate predictive model.

In the pursuit of combating malnutrition, alignment with key United Nations Sustainable Development Goals (SDGs) is crucial. One of the primary targets of this project is to attain SDG 2: Zero Hunger, aiming to eliminate hunger, achieve food security, and promote sustainable agriculture. Additionally, the project contributes to targeting the attainment of SDG 3: Good Health and Well-Being, recognizing the intrinsic link between malnutrition and overall health outcomes. Addressing this global challenge also aligns with SDG 1: No Poverty and SDG 10: Reduced Inequality, acknowledging the interconnected nature of these goals.

# Review of Related Literature
**Malnutrition**

Malnutrition encompasses deficiencies or excesses in nutrient intake, essential nutrient imbalances, or impaired nutrient utilization. The dual challenge of malnutrition involves both undernutrition and overweight/obesity, along with diet-related noncommunicable diseases. Undernutrition manifests through four main forms: wasting (low weight-for-height), stunting (low height-for-age), underweight (low weight-for-age), and micronutrient deficiencies. Wasting typically indicates recent and severe weight loss, often due to insufficient food quantity and quality or prolonged illnesses, posing a higher risk of death in children if untreated. Stunting results from chronic undernutrition associated with factors like poverty, poor maternal health, frequent illness, and inadequate early-life care, limiting children's physical and cognitive development. Underweight is defined as low weight-for-age, and a child classified as underweight may exhibit stunting, wasting, or both. Micronutrient deficiencies involve insufficient essential vitamins and minerals crucial for bodily functions, including enzyme and hormone production essential for growth and development [2].

Malnutrition is accountable for nearly half of all avoidable deaths in children under 5, resulting in the loss of hundreds of thousands of young lives annually due to hunger-related causes. The pandemic's impacts are anticipated to exacerbate this crisis, with nearly 14 million additional children expected to be severely malnourished by the coming year. This projection amounts to 58.9 million young children, nearly the entire population of South Africa, facing life-threatening malnutrition unless urgent global interventions occur. Unfortunately, nutrition has historically received limited attention from country governments and donors. Despite heightened global awareness of the significance of maternal and child nutrition, investments in this critical area have only increased by 7 percent in recent years (since 2015), a far from adequate response to the escalating problem [3].

**Causes of Malnutrition**

Malnutrition is a complex and pervasive issue characterized by a multitude of factors operating across different levels. Immediate causes of malnutrition are linked to insufficient dietary intake and the presence of diseases. This results from a variety of challenges, including food insecurity, inadequate healthcare access, and unsanitary living conditions. Underlying causes of malnutrition are deeply rooted in societal issues such as conflicts, poverty, and gender inequality. These factors contribute to household food insecurity and unfavorable social environments, exacerbating the risk of malnutrition. At a broader level, basic causes involve complex societal dynamics, encompassing human, economic, and organizational resources. Poverty, lack of information, and political instability play significant roles in shaping the landscape of malnutrition. Children, being particularly vulnerable, face additional risks, including preterm birth, diseases, and socio-economic factors. Recognizing the multifaceted nature of these causes is crucial for the development of comprehensive strategies aimed at combating malnutrition on a global scale. Addressing immediate, underlying, and basic causes is essential for effective interventions that can holistically address the intricate web of factors contributing to malnutrition [4]

**Effects of Malnutrition**

According to [5], malnutrition, defined as inadequate nutrition stemming from insufficient food intake or a deficiency in essential nutrients, induces substantial health effects. A well-balanced diet, supplying sufficient calories, protein, and vitamins, plays a pivotal role in sustaining optimal health. Inadequate nutritional intake may result in unintended weight loss, muscle depletion, a reduced body mass index (BMI), and deficiencies in crucial vitamins and minerals. The consequences of malnutrition encompass tangible physical effects, including fatigue, weakness, and compromised recovery from illnesses. Recognizing malnutrition proves challenging due to its gradual onset, with observable signs such as diminished appetite, unplanned weight loss, reduced energy levels, challenges in daily activities, mood alterations, and heightened susceptibility to infections. Timely recognition and intervention, as suggested by research findings, are paramount to mitigating these adverse effects and fostering comprehensive well-being, thereby preventing potential long-term health complications. 

**Malnutrition in the Philippines**

As stated in the article [6], "The State of the World’s Children: Children, Food and Nutrition," illuminate a troubling trajectory in the Philippines, where malnutrition continues to be a pressing concern. As per the report, a notable 33% of children under the age of five exhibit stunted growth, with approximately 7% experiencing underweight conditions, and one-tenth of Filipino adolescents grappling with overweight issues. The documented causes of malnutrition include suboptimal health-seeking behavior, incomplete immunization, inadequate hygiene, and insufficient dietary quantity and quality. The National Nutrition Council (NNC), in accordance with the Philippine Plan of Action for Nutrition (PPAN) 2017-2022, underscores the critical role of the first 1,000 days of life in addressing malnutrition. Despite concerted efforts, the persistently high rates of stunting underscore the necessity for targeted interventions in early childhood nutrition. Noteworthy challenges outlined in the literature review involve subpar rates of exclusive breastfeeding and insufficient nutritional intake for both infants and adolescents. The comprehensive review emphasizes the imminent threats posed by the triple burden of malnutrition to child health, thereby emphasizing the urgency of collaborative endeavors involving government bodies, the private sector, civil society, and various stakeholders to comprehensively tackle the complexities of unhealthy eating practices in the Filipino context. 

# Gathered Data / Dataset

The gathered data on malnutrition, titled "Malnutrition Across the Globe," was accessed using Kaggle. The whole group had agreed to choose this topic because it is one of the most common issues worldwide that needs assessment and resolution. It also has numerous connections to UN SDGs, which can significantly contribute to the achievement of these goals. This topic essentially comprises two downloadable datasets compiled in an Excel file, containing information about malnutrition in every country worldwide. The four broad types of malnutrition, namely wasting, stunting, underweight, and overweight, are also included in the gathered data. All the data included in both datasets are based on surveys conducted in previous years by the United Nations, that is why the information contained herein is real and accurate.

Link of the shared dataset: https://www.kaggle.com/datasets/ruchi798/malnutrition-across-the-globe/data

# Objectives

**1.	 Assess the Global Trends in Childhood Malnutrition**

Identify and analyze trends in malnutrition profiles among children aged 0–59 months worldwide. Consider different types of malnutrition and examine whether cases of malnutrition have decreased or increased over the period indicated.

**2.	Identification of Most Prevalent Forms of Malnutrition**
Determine the most prevalent forms of malnutrition among children aged 0–59 months globally. Focus on severe wasting, wasting, overweight, stunting, and underweight, and analyze the percentage distribution of each type to understand the relative burden of these conditions.**

**3.	Income Classification and Malnutrition Rate****

Explore the correlation between the income classification of countries and the prevalence of malnutrition among children under 5. Investigate whether there are significant differences in the percentage of stunted, overweight, and wasted children based on the income classification of countries.

**4.	Data Quality and Reporting Discrepancies**

Assess the reliability and consistency of malnutrition data reporting across countries. Identify potential challenges and discrepancies in data collection and reporting methods and propose recommendations for improving the accuracy and comparability of global malnutrition statistics.

**5.	Model Evaluation**

To assess the best forming modeling techniques between linear regression, logistic regression, and classification model.

# Conceptual

To achieve the primary goal of training and evaluating the collected data, our approach involves a series of steps illustrated in Figure 1. Initially, the data undergoes a crucial phase of data preprocessing within the data analysis pipeline. This phase encompasses tasks such as handling missing values, eliminating outliers, and scaling features, contributing to a comprehensive understanding of the dataset's characteristics. Following data preprocessing, we proceed to feature selection, underscoring the importance of retaining informative features for precise predictions while discarding irrelevant and redundant information.
Subsequently, the dataset undergoes model training, employing linear regression, logistic regression, and classification models. For linear regression, we select independent and dependent variables for each malnutrition classification, taking income classification as the independent variable. We calculate Root Mean Squared Error (RMSE) and Mean Absolute Error (MAE), visualizing the relationship between the independent and dependent variables. Logistic regression is applied due to the categorical nature of the malnutrition dataset. The dataset is split into training and testing sets to implement logistic regression effectively. Additionally, classification models, namely Support Vector Machine (SVM), Decision Tree, and Random Forest, are utilized.
Finally, in the model evaluation phase, a comparative analysis is conducted to determine the performance of each model technique during training. This comprehensive approach ensures a systematic exploration of various methods, allowing for informed decisions on model selection and optimization.

![image](https://github.com/hanamae-prog/Data-Science-and-AI/assets/137803175/0f1ae4ca-1e31-4bba-a36f-baa32da3d780)


# Data and Results (Visualization)

In conducting the capstone assessment regarding the provision of solutions for Malnutrition, the students explored the performance of several models, including Linear Regression, Logistic Regression, Support Vector Machine (SVM), Decision Tree, and Random Forest.

**Linear Regression:**

Strengths:

Linear regression provides clear and interpretable coefficients for each feature. This means that it can easily understand the impact of each predictor variable on the target variable. Achieved relatively high R2 values for predicting 'Stunting.' The relatively high R2 for predicting 'Stunting' indicates that the linear regression model performed well in explaining the variation in this specific variable.

Weaknesses:

The limited performance on other variables suggests that linear regression might not have been as effective in capturing the relationships for some of the other variables like 'Severe Wasting,' 'Wasting,' 'Overweight,' and 'Underweight.' Another is that outliers can disproportionately influence the slope and intercept of the regression line, potentially impacting the model's accuracy. Which is why it is imperative to eliminate outliers in the dataset before performing any analysis.


Table 1. Linear Regression Testing Results


![image](https://github.com/hanamae-prog/Data-Science-and-AI/assets/137803175/d91018d9-06e0-4d80-be5b-31dcb1a1e4af)







![image](https://github.com/hanamae-prog/Data-Science-and-AI/assets/137803175/d9d7634e-0f36-4641-9222-214c69c15857)








![image](https://github.com/hanamae-prog/Data-Science-and-AI/assets/137803175/7448990b-a7e6-4006-89d8-703a71f5541c)









**Logistic Regression:**

Strengths:
Logistic regression is suitable for binary classification tasks. High overall accuracy (0.93) with balanced precision and recall indicating that the model is effective at making correct predictions on the majority of instances. A balanced precision and recall mean that the model performs well in both correctly identifying positive instances (precision) and capturing all actual positive instances (recall).

Weaknesses:
May not handle complex relationships in the data as effectively. The decision to group the four income classes into two for binary classification using Logistic Regression can simplify the model and make it more interpretable. However, this simplification comes at the cost of potentially losing information present in the original four classes. If the relationships between features and income classes are complex and nonlinear, logistic regression may struggle to capture these nuances effectively.


Table 2. Logistic Regression performance evaluation



![image](https://github.com/hanamae-prog/Data-Science-and-AI/assets/137803175/56e24984-5469-4ab2-8938-da2a7d56230f)






**Support Vector Machine (SVM):**
Strengths:
The SVM model achieved a moderate accuracy of 0.65 on the test dataset. While it is not the highest accuracy among the models used, it suggests a reasonable ability to make correct predictions with potential for improvement. The SVM model also provides flexibility with different kernel functions which are versatile and can handle different types of relationships between features and classes by using various kernel functions and capture more complex data.

Weaknesses:
The SVM model encountered difficulties when dealing with class imbalances in the dataset. Class imbalances occur when the number of instances in different classes is not roughly equal. In the dataset, the model struggled with this imbalance and affected its performance.

Table _. Support Vector Machine (SVM) classification results



![image](https://github.com/hanamae-prog/Data-Science-and-AI/assets/137803175/bb2c8e49-6a4b-4168-94e8-26ee9d5ef540)







**Decision Tree:**

Strengths:
Decision Trees have a straightforward and intuitive structure. The decision-making process is similar to a flowchart which makes it easy to understand with its simple and interpretable model. Decision Trees are capable of capturing complex, non-linear relationships within the data. They can identify decision boundaries that aren't necessarily linear, making them suitable for datasets with intricate patterns.

Weaknesses:
The Decision Tree model used in the dataset achieved an accuracy of 0.46, which is lower than the accuracies of other models. This indicates that for the given dataset, this model might not have been able to capture the underlying patterns as effectively as other models. This model is also sensitive to noise or outliers in the data affecting its performance.


Table 3. Decision Tree classification results




![image](https://github.com/hanamae-prog/Data-Science-and-AI/assets/137803175/d451d969-cf83-4cc7-98f8-9c5942c9ac44)







**Random Forest:**

Strengths:
Random Forest is a group model that builds multiple decision trees and combines their predictions. This group approach often leads to better accuracy compared to individual decision trees, making it a somewhat better model used in this particular dataset. The model aggregates the predictions of multiple trees, where the model tends to generalize well to unseen data, improving the model's overall performance as compared to the Decision Tree model.

Weaknesses:
This model is a group of many decision trees and is more complex than a single decision tree. While it offers improved predictive performance, the interpretability of the model diminishes. Understanding the specific decision-making process of a Random Forest model becomes challenging due to the combined output of numerous trees. 

Table 4. Random Forest classification results


![image](https://github.com/hanamae-prog/Data-Science-and-AI/assets/137803175/08fc03f9-8495-4e6e-90aa-0dbe99648358)







# Conclusion

In conclusion, the exploration of malnutrition datasets has unveiled critical insights that a distinct correlation is evident between the classification of income and the prevalence of malnutrition. Generally, nations with lower income levels exhibit higher rates of stunting, wasting, and underweight in comparison to their higher-income counterparts. Specifically, low-income countries experience stunting rates that are five times more pronounced than those in high-income countries. However, the manifestation of overweight cases in high-income contexts adds a layer of complexity to the issue, necessitating attention to both undernutrition and overnutrition across all income strata.

While strides have been made globally in mitigating stunting, the persistent challenge of wasting and the emergence of overweight create a nuanced and intricate scenario. Effectively addressing childhood malnutrition demands a comprehensive strategy that considers income disparities, access to nutritious food, healthcare provisions, and proper sanitation. Further investigation is imperative to discern the intricate factors steering these trends, allowing for the implementation of targeted interventions tailored to specific regions and income categories.


In contrast, concerning the most effective model technique, Logistic Regression proved to be the superior model, surpassing others in terms of accuracy, precision, recall, and F1-score. Linear models, including Linear Regression, successfully captured clear relationships. Support Vector Machines faced challenges with class imbalances, while Decision Tree struggled with accuracy due to dataset complexity. Though more accurate, Random Forest traded off interpretability.

Moreover, to improve performance, feature engineering is advised, involving the creation of new variables or extraction of meaningful information. Continuous optimization is crucial for sustained enhancement. The holistic analysis provides insights into global trends, country-specific variations, malnutrition prevalence, socio-economic correlations, and model evaluations. These findings inform evidence-based interventions and policies for addressing childhood malnutrition globally.

# References

[1] 	"World Health Organization," 20 December 2023. [Online]. Available: https://www.who.int/news-room/fact-sheets/detail/malnutrition. [Accessed 11 January 2024].

[2] 	"World Health Organization," [Online]. Available: https://www.who.int/health-topics/malnutrition#tab=tab_1. [Accessed 11 January 2024].

[3] 	"Bread For The World," 23 August 2021. [Online]. Available: https://www.bread.org/article/global-malnutrition-fact-sheet-2021/. [Accessed 11 January 2024].

[4] 	T. L. Ersado, "Causes of Malnutrition," in Combating Malnutrition throrugh Sustainable Approaches, IntechOpen, 2021. 

[5] 	"NHS Inform," 21 November 2023. [Online]. Available: https://www.nhsinform.scot/illnesses-and-conditions/nutritional/malnutrition/#:~:text=tiredness%20or%20low%20energy%20levels,feelings%20of%20lethargy%20and%20depression . [Accessed 19 January 2024].

[6] 	"UNICEF," UNICEF, 16 October 2019. [Online]. Available: https://www.unicef.org/philippines/press-releases/unicef-many-children-and-adolescents-philippines-are-not-growing-healthily. [Accessed 19 January 2024].

