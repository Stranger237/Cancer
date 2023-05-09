# Cancer
## Our customers
Our customers are medical centers, diagnostic centers 
## Value proposition of our project
Such a method will help reduce the workload of a second specialist while examining a patient. AI has a higher sensitivity in detecting cancer compared to live specialists, especially in the case of studies of breasts with a large fat layer (90% vs. 78%)
## Our partners, vendors,etc.
Partners: Research centers, hospitals, health centers
Vendors: There is no need for vendors, we can sell the product ourselves
### Objective
We are going to recognise mammography images for cancer. The model must answer the question:  "What type of tumour is this (benign, malignant)?
### Our model
For the recognition task, convolutional neural networks can be used
CNNs are powerful for analyzing images because pattern-specific filters can preserve the picture’s spatial features. CNNs often outperform dense neural network methods because fully connected architectures flatten input images, overlooking vital spatial patterns. We used VGG19
### Our data
The data is images and labels / annotations for mammography scans. More about the database can be found at MIAS. The 'Preview' kernel shows how the Info.txt and PGM files can be parsed correctly.
The dataset originally has 332 grayscale mammogram images sized at 1024x1024. There are 6 categories of abnormalities classified by severity as either Benign (B) or Malign (M). Normal scans, i.e. those absent from abnormalities, were arbitrarily given the value (A) for classification purposes.
The data is stored as tfrecords files for TensorFlow
### Our metrics
The ROC-AUC is a more informative metric, as it allows readers to compare the true-positive and falsepositive rates. Researchers have recently implemented complex CNN block combinations like squeeze-excitation and attention networks to enhance model performance.

### Benifits for customers
1. Improved accuracy: AI algorithms can analyze mammograms with greater precision and identify subtle changes that may be missed by human radiologists, leading to earlier detection of breast cancer and improved patient outcomes.
2. Increased efficiency: AI can help reduce the workload of radiologists, improving overall efficiency in the healthcare system. This can lead to faster diagnoses and treatment for patients.
3. Cost savings: By reducing the need for additional imaging tests and follow-up appointments, AI can help save healthcare costs for patients and providers.
4. Better patient outcomes: Early detection of breast cancer can lead to better patient outcomes, including improved survival rates and less invasive treatment options.
5. Reduced human error: AI can help reduce the potential for missed or inaccurate breast cancer detection in mammograms due to human error or limitations. This can improve the reliability and accuracy of breast cancer screening programs.

### The business effect of our model’s missprediction
The cost of misprediction by using AI in mammography can also vary depending on the context and consequences of the misprediction. In the context of mammography, misprediction could result in missed diagnoses or false positives, leading to delayed or unnecessary treatments, emotional distress for patients, and potentially even life-threatening consequences if cancer is not detected early enough. This could also lead to increased healthcare costs and decreased trust in AI technology. Therefore, it is crucial to carefully evaluate and validate AI algorithms before implementing them in clinical practice to minimize the risk of misprediction.

Value or profit of using AI in mammography can be measured in several ways. One way is to evaluate the accuracy and efficiency of AI algorithms in detecting breast cancer compared to traditional mammography methods. This can lead to earlier detection of cancer, reduced healthcare costs, and improved patient outcomes. Another way is to assess the potential cost savings from reducing unnecessary biopsies and treatments resulting from false positives. Additionally, AI can improve workflow efficiency, allowing radiologists to focus on more complex cases and increasing patient throughput. These factors can all contribute to the overall value and profitability of using AI in mammography.

### Results
Accuracy: 0.9755
Precision: 0.9756
Recall: 0.9755
F1 Score: 0.9755
ROC AUC Score: 0.9949
Cohen Kappa Score: 0.9508
		Classification Report:
               precision    recall  f1-score   support

           B       0.98      0.98      0.98       418
           M       0.97      0.97      0.97       359

    accuracy                           0.98       777
   macro avg       0.98      0.98      0.98       777
weighted avg       0.98      0.98      0.98       777

