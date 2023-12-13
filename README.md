# Could automation strategies be utilised to classify undiagnosed heart related diseases? & Do chest related pains have any direct correlation to the chances an individual could have a heart attack?

## Motivation of Study
The project has utilised the means of supervised learning which corelates known data of different inputs and correct outputs provided by a data scientist/analytic(Reddy.P,2018)as for machine learning algorithms to learn from the training data as to classify/predict outputs in the future from unseen testing data(Chen.D,2021). The provided dataset for this project has utilised 303 real patient data of individuals who are classified of either having a low chance of heart disease/attacks[0] or a high chance of heart disease/attacks1which means the project will require ML-algorithms capable of classification as classification algorithms are designed to assign the unseen testing data into predict/assign sets of data into a specific category(Taha.B,2019).

Therefore, this project will utilise ML as to predict if unseen data[testing-data] via the collected data from the users age, sex, chest-pain-type[cp], trestbps, chol, restecg, thalach, thal, exang, oldpeak, slp and number-of-major-vesselscaare classified as having heart disease/attacks or not as Heart disease has demonstrated serious concerns for the NHS as during 2022 as the UK has diagnosed 1.5 million individuals with heart related disorders whilst Every week in the UK at least 12 young people die from an undiagnosed heart condition(British Heart Foundation,2022)whilst medical professionals of the World Health Organisation are still only able to successfully diagnose 67% of individuals with heart related diseases(Kirubha.V,2016)Therefore, whilst as my ancestral background[fathers side] have had a history of heart related problems then as the enhancement of software engineering has enhanced the field of data analysis(Arpteg.A,2018)especially in providing new opportunities to the field of medical science(Kushwaha.P,2021)I.E.Machine learning has low become a viable tool towards the classification if an individual has Alzheimer’s disease(Khan.P,2021)

## Analytical Question
The main reasoning behind this project is to determine if such automation strategies could be utilised in the near future to detect, if possible, if individuals are susceptible to and/or have undiagnosed heart related diseases from their medical records alone as to allow the NHS to conduct pre-measurements and/or warnings to prevent any unnecessary future fatalities

However, Throughout the project then I am also hoping to determine if chest related pains have any direct correlation to the chances an individual could have a heart attack as due to my stated ancestral background being susceptible to heart related diseases, then this has exacerbated my health-related fears and hypochondria even during the most benign chest pains.

Therefore, during the project then I am also hoping to determine if chest related pains have any direct correlation to the chances an individual could have a heart attack.

Additionally, through EDA it is hoped to determine what chest pain type are more likely linked to heart attack sufferers

## Methods
In this study then in order to determine if machine learning and automation strategies can be utilised as an efficient means towards classifying undiagnosed heart related diseases/attack sufferers then I will be primarly using SVM whilst comparing SVM to different supervised machine learning algorithms such as Logistic Regression, decision trees, Random Forests, KNN and SVM which are some of the most common tools for classification problems.

The models will be compared via their accuracy and confusion matrix visualisations to determine the most appropriate model with the least false positive/negative predictions/rates(Ohsaki.M,2017)as false-positives are misclassifications where predictions state the set-of-data is positive[heart-disease]when the actual result is negative[no-heart-disease]whilst false-negatives are misclassifications where predictions state the set-of-data is negative[no-heart-disease]when the actual result is negative(heart-disease)(Zorkadis.V,2005)

Only after the highest accuracy model is selected that further proof can be made to determine if chest related pains have any direct correlation to heart related diseases/attacks by performing one dimensional tests where chest pain is the only input as to check the accuracy of predictions via only one input. However, to test the direct importance of the feature[chest-pain] then permutation importance will also be utilised to calculate the error rate of the model when the value in each column is changed/shuffled. If the error-rate significantly increased when chest-pain then it is deemed as important(Altmann.A,2010).However, EDA will also be conducted as to further show if chest pains have any correlation to heart disease whilst also being utilised to determine what chest pain type are more likely linked to heart attack sufferers.

## Conclusion

### Conclusion 1: Could automation be utilised in the near future to detect if possible, individuals are susceptible to and/or have undiagnosed heart related diseases
The results have proven my hypothesis that SVM would be the most efficient model as SVM has received the highest accuracy out of all models at 93.75%. However, it has been surprising that the other models thought to have failed have also score particularly high as even the least effective model AKA Decision Trees, scored 84.375%. Therefore, In theory then from the conclusions made from the project then machine learning and automation could most definitely allow for efficient classifications to determine if an individual is of risk of suffering a heart attack as the project has demonstrated that mostly all the machine learning algorithms have presented high accuracy results with very low false positive and/or false negative rates.

However, due to the risks false positive/negatives then even though all models did considerably well then due to the sensitive nature of medical care then due to the risks of false negatives making the doctor believe the patient does not require any observations/care for heart attacks when in actuality the patient is at risk of a heart attack then this could result in delayed care or even death(Waqar.M,2021). However, false positives also pose a risk as this will result in the doctor believing a patient is at risk of a heart attack from the predictions made from the machine learning algorithm when the patient is actually healthy which could allow in inappropriate appointments being made which could further cause funding and availability strain to the NHS and other sick patients(Ramesh.G,2021)

Therefore, the SVM model should be chosen with the highest accuracy and the lowest false-positive/false-negative rates. However, as there are always risks of positive/negative as even in this example then the SVM experienced one false positive and three false negatives then this suggests that such automation strategies should only be utilised as a tool by the doctors/GP's and not as a replacement(Kim.G,2021)

However, for this to work in practice then due to the small size of the dataset then there are significantly higher chances of overfitting(Kim.H,2019)as if such a dataset was to be utilised in the future on real patient data then there could be a much higher chance of false positives/negatives as unique data noise/outliers may not be classified correctly classified if the model is trained/overfitted to a specific range/value(Montesinos.O,2022)In example then due to data collection bias of the chosen dataset has collected more data of individuals of the age of 60 with a higher ratio of having a lower chance of heart attack then this will increase the risks of false positive/negatives as in the real world then elderly individuals are known to be more susceptible to heart related diseases(Yousuf.H,2021)

Therefore, in future implementations them machine learning and automation can most definitely be utilised to detect heart related diseases but only if the data collection sample includes data that represents the real world from real patient examples to reduce the risks of overfitting and ensuring false positive/negative rates are reduced.

### Conclusion 2: Are chest related pains have any direct corolation to the chances an individual could have a heart attack
From the results found from the EDA then it has been concluded that Analysis on Chest Pain has concluded that chest Pain does seem to have a strong correlation with heart related diseases as all chest pains such as [1=typical-angina]/[2=atypical-angina]/[3=non-anginal-pain] have a much higher ratio of people who at risk of heart attacks compared to people are not at risk of heart related problems/attacks.

Therefore, SVM has further shown its effectiveness as through analysis conducted towards predicting the output with just one input then it has been discovered that chest related pains had the highest accuracy of 81.25% whilst the lowest/least correlated input/feature were Sex and Fbs with accuracies of only 0.546875% whilst this was further proven as the utilisation of SVM and permutation importance has determined that chest pain is one of [if not the best] best colorations indicating an individual is at the risk of having a heart attack along with other features/columns such as caa and thall.

Additionally, through EDA then through the visualisation process it has been determined that the chest pain type with the highest risk of a heart attack is atypical angina[2] which demonstrates, as scary as it may seem, that any signs of chest pains should be taken with 100% seriousness as even though atypical angina symptoms doesn't cover pressure or squeezing when the heart doesn't get the required amount of oxygenated blood(DeVon.H,2020)then since non-anginal and atypical angina pains are still correlated with many heart related attacks[atypical angina being the highest] then this suggests that if any patient indicates symptoms relating to chest related pain then they should quickly be referred to a doctor/GP for a check-up.

However, in the future then as there are still some risks/chances that individuals with little to no symptoms/pains[asymptomatic[0]] could still have heart attacks then even with the strong correlation then chest-pain in itself cannot be utilised by itself to determine if somebody it at risk of a heart attack and must be compared to other factors as from SVM then even though CP by itself had high accuracy by itself then he overall accuracy significantly decreased by 11.6%

## References
Arpteg, A. et al. (2018) ‘Software Engineering Challenges of Deep Learning’, 2018 44th Euromicro Conference on Software Engineering and Advanced Applications (SEAA), pp. 50–59. doi:10.1109/SEAA.2018.00018.

British Heart Foundation (2022) UK Factsheet: Our vision is a world free from fear of heart and circulatory diseases Available At: https://www.bhf.org.uk/what-we-do/our-research/heart-statistics [Accessed: 08/03/2022]

Chen, D. et al. (2021) ‘Self-Supervised Learning For Few-Shot Image Classification’, IEEE Access [Preprint]. Available at: http://arxiv.org/abs/1911.06045 (Accessed: 9 May 2022).

DeVon, H.A., Mirzaei, S. and Zègre‐Hemsey, J. (2020) ‘Typical and Atypical Symptoms of Acute Coronary Syndrome: Time to Retire the Terms?’, Journal of the American Heart Association, 9(7), p. 4. doi:10.1161/JAHA.119.015539.

Jay (2021) ‘Description of features’ Available At: https://www.kaggle.com/datasets/rashikrahmanpritom/heart-attack-analysis-prediction-dataset/discussion/234843 [Accessed: 09/05/2022]

Khan, P. et al. (2021) ‘Machine Learning and Deep Learning Approaches for Brain Disease Diagnosis: Principles and Recent Advances’, IEEE Access, 9, pp. 37622–37655. doi:10.1109/ACCESS.2021.3062484.

Kim, G.H., Sung, E.-S. and Nam, K.W. (2021) ‘Automated laryngeal mass detection algorithm for home-based self-screening test based on convolutional neural network’, BioMedical Engineering OnLine, 20(1), p. 51. doi:10.1186/s12938-021-00886-4.

Kirubha, V. and Priya, S.M. (2016) ‘Survey on Data Mining Algorithms in Disease Prediction’, International Journal of Computer Trends and Technology, 38(3), pp. 124–128. doi:10.14445/22312803/IJCTT-V38P122.

Kushwaha, P.K. and Kumaresan, M. (2021) ‘Machine learning algorithm in healthcare system: A Review’, in 2021 International Conference on Technological Advancements and Innovations (ICTAI). 2021 International Conference on Technological Advancements and Innovations (ICTAI), Tashkent, Uzbekistan: IEEE, pp. 478–481. doi:10.1109/ICTAI53825.2021.9673220.

Macina.J (2017) ‘Determining the most contributing features for SVM classifier in sklearn’ Available At: https://stackoverflow.com/questions/41592661/determining-the-most-contributing-features-for-svm-classifier-in-sklearn [Accessed: 09/05/2022]

Montesinos López, O.A., Montesinos López, A. and Crossa, J. (2022) Multivariate Statistical Machine Learning Methods for Genomic Prediction. Cham: Springer International Publishing (1). doi:10.1007/978-3-030-89010-0.

Ohsaki, M. et al. (2017) ‘Confusion-Matrix-Based Kernel Logistic Regression for Imbalanced Data Classification’, IEEE Transactions on Knowledge and Data Engineering, 29(9), pp. 1806–1819. doi:10.1109/TKDE.2017.2682249.

Rahman.R (2021) ‘Heart Attack Analysis & Prediction Dataset’, Available At: https://www.kaggle.com/datasets/rashikrahmanpritom/heart-attack-analysis-prediction-dataset [Accessed: 09/05/2022]

Ramesh, G. et al. (2021) ‘Improving the accuracy of heart attack risk prediction based on information gain feature selection technique’, Materials Today: Proceedings, p. S2214785320397649. doi:10.1016/j.matpr.2020.12.079.

Reddy, P., Viswanath, P. and Reddy, E. (2018) ‘Semi-supervised learning: a brief review’, International Journal of Engineering & Technology, 7(1.8), p. 81. doi:10.14419/ijet.v7i1.8.9977.

Taha, B. and Shoufan, A. (2019) ‘Machine Learning-Based Drone Detection and Classification: State-of-the-Art in Research’, IEEE Access, 7, pp. 138669–138682. doi:10.1109/ACCESS.2019.2942944.

Waqar, M. et al. (2021) ‘An Efficient SMOTE-Based Deep Learning Model for Heart Attack Prediction’, Scientific Programming. Edited by M.-C. Chen, 2021, pp. 1–12. doi:10.1155/2021/6621622.

Yousuf, H. et al. (2021) ‘A media intervention applying debunking versus non-debunking content to combat vaccine misinformation in elderly in the Netherlands: A digital randomised trial’, EClinicalMedicine, 35, p. 100881. doi:10.1016/j.eclinm.2021.100881.
