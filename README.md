# Ear-Disease-Clasification

## Introduction
Hearing disorders are a serious global health issue, affecting quality of life and human productivity. The World Health Organization (WHO) reported that in 2021, approximately 430 million people worldwide required hearing rehabilitation services, with projections indicating a significant increase to 2.5 billion people by 2050.
In Indonesia, the diagnosis and treatment of hearing disorders are hindered by several factors:
-	Uneven distribution of ENT (Ear, Nose, and Throat) specialists, especially in remote areas.
-	Limited access to specialist services and adequate diagnostic equipment.
-	The "invisible handicap" nature of hearing disorders, often causing patients to be unaware of their condition.

Accurate and rapid diagnosis is key in addressing hearing disorders. However, conventional diagnostic methods require considerable time for result interpretation by doctors. Therefore, there is a need for technology that can assist doctors in identifying types of ear diseases in real-time.

This research proposes the use of Xception and MobileNet-V2 architecture models with the implementation of Bayesian optimizer for the classification of 20 types of ear diseases. The aim is to improve the accuracy and speed of diagnosis, enabling more precise and effective prevention and treatment actions.

Using a dataset of 1,101 images from the University of Mataram Hospital, this study is expected to make a significant contribution to improving the quality of ear health services, especially in areas with limited access to ENT specialists.

By leveraging advanced machine learning techniques, this research seeks to address the challenges in ear disease diagnosis, potentially reducing the global burden of hearing disorders and improving access to quality healthcare in underserved regions.

## Dataset Sample

<table>
  <tr>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Acute%20Otitis%20Media%20%E2%80%93%20Hypermic/2016-10-31T19-00-45.jpg" width="250"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Acute%20Otitis%20Media%20%E2%80%93%20Perforation/2016-12-22T20-02-30.jpg" width="250"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Acute%20Otitis%20Media%20%E2%80%93%20Resolution/2017-05-08T19-18-07.jpg" width="250"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Acute%20Otitis%20Media%20%E2%80%93%20Supporation/2017-02-22T19-30-54.jpg" width="250"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Acute%20Otitis%20Media%20%E2%80%93%20Turbal%20Occlusion/2017-02-20T19-48-42.jpg" width="250"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Aerotitis%20Barotrauma/2017-10-09T19-35-44.jpg" width="250"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Bullos%20Myringitis/2016-10-28T17-42-44.png" width="250"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Cerumen/2016-11-17T20-20-02%20-%20Copy.jpg" width="250"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Chronic%20Suppurative%20Otitis%20Media%20-%20Resolution/2017-05-08T19-17-35.jpg" width="250"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Chronic%20Suppurative%20Otitis%20Media%20-Safe%20Type/2016-10-26T19-33-01.png" width="250"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Chronic%20Suppurative%20Otitis%20Media%20%E2%80%93%20Unsafe%20Type/2016-11-02T19-07-46.jpg" width="250"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Corpus%20Alienum/2017-01-23T19-08-54.jpg" width="250"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Diffuse%20Exterenal%20Otitis/2016-10-27T19-19-11.png" width="250"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Furuncular%20External%20Otitis/2017-05-15T19-48-30.jpg" width="250"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Normal%20Tympanic%20Membrane/2016-10-31T18-19-18.jpg" width="250"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Normal/N1.jpg" width="250"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Otitis%20Media%20with%20Effusion/2017-03-03T20-47-26.jpg" width="250"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Otomycosis/2016-10-26T18-51-26.png" width="250"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Tympanic%20Membrane%20Perforation/2016-11-30T19-56-04.jpg" width="250"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Tympanosclerosis/2016-10-26T19-33-36%20-%20Copy.png" width="250"></td>
  </tr>
  <tr>
    <td align="center">Acute Otitis Media - Hypermic</td>
    <td align="center">Acute Otitis Media - Perforation</td>
    <td align="center">Acute Otitis Media - Resolution</td>
    <td align="center">Acute Otitis Media - Suppuration</td>
    <td align="center">Acute Otitis Media - Turbal Occlusion</td>
    <td align="center">Aerotitis Barotrauma</td>
    <td align="center">Bullos Myringitis</td>
    <td align="center">Cerumen</td>
    <td align="center">Chronic Suppurative Otitis Media - Resolution</td>
    <td align="center">Chronic Suppurative Otitis Media - Safe Type</td>
    <td align="center">Chronic Suppurative Otitis Media - Unsafe Type</td>
    <td align="center">Corpus Alienum</td>
    <td align="center">Diffuse Exterenal Otitis</td>
    <td align="center">Furuncular External Otitis</td>
    <td align="center">Normal Tympanic Membrane</td>
    <td align="center">Normal</td>
    <td align="center">Otitis Media with Effusion</td>
    <td align="center">Otomycosis</td>
    <td align="center">Tympanic Membrane Perforation</td>
    <td align="center">Tympanosclerosis</td>

  </tr>
</table>

## Model Building

This research applies the transfer learning method to classify ear diseases. It involves using a pre-trained model and applying it to a new task: ear disease classification. Transfer learning transfers most network layers from a model previously trained on ImageNet (with 1.4 million images across 1000 classes) to a model for ear disease classification, followed by new fully-connected layers that classify these features into new classes.

Additional models are added to process the output from pre-trained models (MobileNet-V2 and Xception). Pre-trained models have many layers that process image inputs and generate features; the added model will process the features produced by the pre-trained model for classification tasks. The following layers are added:

-	Adding the pre-trained model as the basis for the new model
-	Global Average Pooling
-	Dense
-	ReLU Activation
-	Dropout
-	Softmax Activation
-	Output Dense

Adding classification layers from the additional model can improve performance as these layers help the model learn more complex and abstract features from the data, reduce overfitting, and improve model generalization. However, this approach relies on previously trained deep learning algorithms, requiring substantial computational resources for training and inference, which can be a barrier in resource-limited environments and low-specification devices.

One solution to address the weakness of dependence on pre-trained deep learning algorithms that require substantial computational resources is to perform careful hyperparameter search to achieve an efficient balance between effective learning from available data and preventing overfitting.

The steps in performing the Bayesian optimizer technique to search for hyperparameters in this research are as follows:
Load data and ensure images are sized 224x224 for MobileNet-V2 and 229x229 for Xception, with pixel normalization from -1 to 1. This preprocessing step ensures input images conform to the pre-trained models' defaults.

Define the pre-trained model as the base model and add additional layers similar to the previous scenario: GlobalAveragePooling2D, dense, dropout, and output dense.

Define the search space for three hyperparameters: number of units in the dense layer (32 to 256), dropout rate (0.2 to 0.5), and learning rate (0.0001 to 0.01).

Define the objective function: the process of training and evaluating the model by training for 10 epochs and calculating validation accuracy. The objective function aims to minimize the validation loss, thereby maximizing validation accuracy.

Perform optimization using Gaussian Process for Bayesian Optimizer. The optimization process applies 50 evaluations to find the best hyperparameters. For the first 10 parameter sets, the algorithm will randomly select values from the ranges specified in the search space.

Use the results from these 10 evaluations to build an initial Gaussian Process model, which becomes the basis for the search in the subsequent 40 iterations.

The ultimate goal of this optimization is to find the combination of hyperparameters in the search space (dense units, dropout rate, learning rate) that yields the highest validation accuracy.

This process allows for efficient exploration of the hyperparameter space, balancing between exploration of new areas and exploitation of promising regions, to find the optimal configuration for the model.

### MobileNet-V2 Hyperparameters

The hyperparameter search for MobileNet-V2 resulted in the best hyperparameters as shown in Table

| **Hyperparameter** | **Value**                   |
|--------------------|-----------------------------|
| Unit Dense         | 174                         |
| Dropout Rate       | 0.2                         |
| Learning Rate      | 0.003103753471420176        |

<table>
  <tr>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Hyperparameter%20Optimizer/MobileNet-V2/Dropout%20Rate.png" width="500"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Hyperparameter%20Optimizer/MobileNet-V2/Learning%20Rate.png" width="500"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Hyperparameter%20Optimizer/MobileNet-V2/Unit%20Dense.png" width="500"></td>
  </tr>
  <tr>
    <td align="center">Dropout Rate</td>
    <td align="center">Learning Rate</td>
    <td align="center">Unit Dense</td>
  </tr>
</table>

### Xception Hyperparameters

After 50 iterations with 10 epochs, the best hyperparameters for Xception were found as shown in Table

| **Hyperparameter** | **Value**                   |
|--------------------|-----------------------------|
| Unit Dense         | 209                         |
| Dropout Rate       | 0.2                         |
| Learning Rate      | 0.0018277161121728472       |

<table>
  <tr>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Hyperparameter%20Optimizer/Xception/Dropout%20Rate.png" width="500"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Hyperparameter%20Optimizer/Xception/Learning%20Rate.png" width="500"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Hyperparameter%20Optimizer/Xception/Unit%20Dense.png" width="500"></td>
  </tr>
  <tr>
    <td align="center">Dropout Rate</td>
    <td align="center">Learning Rate</td>
    <td align="center">Unit Dense</td>
  </tr>
</table>

## Result Analysis

The model testing applied three scenarios:
- Classification using a model with a dataset split ratio of 60:20:20, setting the hyperparameters for the classification layers (scenario 1)
- Testing by implementing hyperparameter search (scenario 2)
- Testing the model with a dataset split ratio of 80:20 (scenario 3)

The best performance achieved by the model in each scenario is summarized in Table.

| **Scenario** | **Epoch** | **AUC Training** | **Loss Training** | **AUC Validation** | **Loss Validation** |
|--------------|-----------|------------------|-------------------|--------------------|---------------------|
| **1**        |           |                  |                   |                    |                     |
| MobileNet-V2 | 93        | 0.987            | 0.771             | 0.912              | 1.742               |
| Xception     | 96        | 0.975            | 1.050             | 0.924              | 1.676               |
| **2**        |           |                  |                   |                    |                     |
| MobileNet-V2 | 17        | 0.991            | 0.597             | 0.922              | 1.671               |
| Xception     | 4         | 0.990            | 0.618             | 0.924              | 1.687               |
| **3**        |           |                  |                   |                    |                     |
| **MobileNet-V2** | **96** | **0.989**        | **0.706**         | **0.931**          | **1.550**           |
| Xception     | 100       | 0.982            | 0.925             | 0.913              | 1.729               |

A summary of the model testing against the test data is also provided in Table 4.33, which contains the average values of accuracy, precision, recall, and f1-score for each model testing scenario.

| **Scenario**   | **Accuracy** | **Precision** | **Recall** | **F1-score** |
|----------------|--------------|---------------|------------|--------------|
| **1**          |              |               |            |              |
| MobileNet-V2   | 0.907        | 0.122         | 0.118      | 0.119        |
| **Xception**   | **0.911**    | **0.166**     | **0.166**  | **0.151**    |
| **2**          |              |               |            |              |
| MobileNet-V2   | 0.911        | 0.132         | 0.136      | 0.131        |
| Xception       | 0.907        | 0.110         | 0.106      | 0.098        |
| **3**          |              |               |            |              |
| MobileNet-V2   | 0.907        | 0.112         | 0.109      | 0.108        |
| Xception       | 0.911        | 0.126         | 0.157      | 0.136        |

## Conclusion

This study analyzes the effectiveness of MobileNet-V2 and Xception models in ear disease classification, using various test scenarios. Initially, Xception performed better with a dataset ratio of 60:20:20, but after hyperparameter optimization using Bayesian optimizer, MobileNet-V2 surpassed Xception. Consistently, the 60:20:20 dataset sharing ratio proved more effective than 80:20 for both models. However, all scenarios faced significant challenges in the form of large gaps between training and validation performance, indicating generalization issues. Despite the high accuracy achieved, both models showed weaknesses in detecting specific disease classes, with a tendency to predict negatively for the majority of cases. The main factor behind this problem is dataset imbalance, where the models are only able to detect true positives in classes with a sufficiently large number of samples (more than 31 images).

Based on the results of this study, future suggestions are to address dataset imbalance in model training by collecting additional data for minority classes or through a hierarchical approach by grouping similar classes for stepwise classification, for example, binary normal/abnormal classification followed by multi-class classification for specific disease types. Implement a sampling strategy using proven methods to divide the dataset into training, validation and testing sets to ensure balanced representation in each set.Continue the exploration of hyperparameter search on pre-trained models for more significant improvement in classification performance.

## References
- https://journal.uwhs.ac.id/index.php/jitk/article/view/363
- http://journal.scientic.id/index.php/sciena/issue/view/8
- http://apps.who.int/bookorders.
- https://www.cell.com/heliyon/fulltext/S2405-8440(24)02617-3
- http://3.8.6.95/ijcs/index.php/ijcs/article/view/3254
- https://www.thelancet.com/article/S2352-3964(19)30431-1/fulltext
- https://www.mdpi.com/2306-5354/10/8/979
- https://keras.io/api/applications/
- https://onlinelibrary.wiley.com/doi/abs/10.1002/lary.29302


## Poster
<table>
  <tr>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Poster.png" width="700"></td>
  </tr>
</table>
