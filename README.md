# Cancer
## Who are your customers?
Our customers are medical centers, diagnostic centers 
## What is the value proposition of your project?
Such a method will help reduce the workload of a second specialist while examining a patient. AI has a higher sensitivity in detecting cancer compared to live specialists, especially in the case of studies of breasts with a large fat layer (90% vs. 78%)
## Who are your partners, vendors,etc.?
Partners: Research centers, hospitals, health centers
Vendors: There is no need for vendors, we can sell the product ourselves
## Specify your project in terms of Deep Learning:
What's your learning objective?(What do you predict/classify/generate?)
We are going to recognise mammography images for cancer. The model must answer the question: "Is there cancer in the picture?"
What's your model? Justify your choice.
For the recognition task, convolutional neural networks can be used
CNNs are powerful for analyzing images because pattern-specific 
filters can preserve the picture’s spatial features. CNNs often outperform dense neural network methods because fully connected architectures flatten input images, overlooking vital spatial patterns. 

What is your data? What is the source of your data? (Modality, features, shape, and anything you see is vital about your data).

Which metrics do you choose?Justify your answer.
The ROC-AUC is a more informative 
metric, as it allows readers to compare the true-positive and falsepositive rates. Researchers have recently implemented complex CNN block combinations like squeeze-excitation and attention networks to enhance model performance.
What is the business effect of your model’s false predictions?
False prediction can lead to misdiagnosis of very serious and life-threatening conditions. In our case false prediction can lead to patient’s death and result in lawsuits against us. 
Specify the training infrastructure you might need.
