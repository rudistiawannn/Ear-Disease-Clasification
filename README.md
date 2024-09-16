# Ear-Disease-Clasification

# Introduction
Hearing disorders are a serious global health issue, affecting quality of life and human productivity. The World Health Organization (WHO) reported that in 2021, approximately 430 million people worldwide required hearing rehabilitation services, with projections indicating a significant increase to 2.5 billion people by 2050.
In Indonesia, the diagnosis and treatment of hearing disorders are hindered by several factors:
-	Uneven distribution of ENT (Ear, Nose, and Throat) specialists, especially in remote areas.
-	Limited access to specialist services and adequate diagnostic equipment.
-	The "invisible handicap" nature of hearing disorders, often causing patients to be unaware of their condition.

Accurate and rapid diagnosis is key in addressing hearing disorders. However, conventional diagnostic methods require considerable time for result interpretation by doctors. Therefore, there is a need for technology that can assist doctors in identifying types of ear diseases in real-time.

This research proposes the use of Xception and MobileNet-V2 architecture models with the implementation of Bayesian optimizer for the classification of 20 types of ear diseases. The aim is to improve the accuracy and speed of diagnosis, enabling more precise and effective prevention and treatment actions.

Using a dataset of 1,101 images from the University of Mataram Hospital, this study is expected to make a significant contribution to improving the quality of ear health services, especially in areas with limited access to ENT specialists.

By leveraging advanced machine learning techniques, this research seeks to address the challenges in ear disease diagnosis, potentially reducing the global burden of hearing disorders and improving access to quality healthcare in underserved regions.

# Dataset

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
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Otomycosis/2016-10-26T18-51-26.png" width="250"></td>
    <td><img src="https://github.com/rudistiawannn/Ear-Disease-Clasification/blob/main/Ear%20Disease%20Dataset%20Sample/Tympanosclerosis/2016-10-26T19-33-36%20-%20Copy.png" width="250"></td>
  </tr>
  <tr>
    <td align="center">Acute Otitis Media Hypermic</td>
    <td align="center">Acute Otitis Media Perforation</td>
    <td align="center">Acute Otitis Media Resolution</td>
    <td align="center">Acute Otitis Media Suppuration</td>
    <td align="center">Acute Media Turbal Occlusion</td>
    <td align="center">Aerotitis Barotrauma</td>
    <td align="center">Bullos Myringitis</td>
    <td align="center">Cerumen</td>
    <td align="center">Chronic Suppurative Otitis Media Resolution</td>
    <td align="center">Chronic Suppurative Otitis Media Safe Type</td>
    <td align="center">Chronic Suppurative Otitis Media Unsafe Type</td>
    <td align="center">Corpus Alienum</td>
    <td align="center">Diffuse Exterenal Otitis</td>
    <td align="center">Furuncular External Otitis</td>
    <td align="center">Normal Tympanic Membrane</td>
    <td align="center">Normal</td>
    <td align="center">Otitis Media with Effusion</td>
    <td align="center">Otomycosis</td>
    <td align="center">Otomycosis</td>
    <td align="center">Tympanosclerosis</td>

  </tr>
</table>
