# SUD-Dataset
Silvia María González Collazo, Jesús Balado, Iván Garrido, Javier Grandío, Rabbia Rashdi, Elisavet Tsiranidou, Pablo del Río-Barral, Erik Rúa, Iván Puente and Henrique Lorenzo
## Introduction
The Santiago Urban Dataset (SUD) is a large labelled point cloud database acquired with MLS and HMLS scaners in Santiago de Compostela (Spain). Both data were georeferenced and labelled into eight main classes; *road, sidewalk, curb, buildings, vehicles, vegetation, pole-like elements* and *others*. Therefore, it is presented a datased which distinguish the ground urban elements and combines MLS with HMLS 3D point clouds.
This dataset covers around 2 km of streets, and contains fourteen segments of six urban streets.

![Esto es una imagen](Image_1.png)

Given the existence of two data sources, three tests with their corresponding three training sessions were performed: one considering only the MLS point clouds, another one considering only the HMLS point clouds and a third one considering both MLS and HMLS point clouds. The dataset was divided into training, validation and test sets. The following table shows the accuracies obtained for each training session.

|                | Road | Sidewalk | Curb | Building | Vehicles | Vegetation | Poles |Others |
| ---            | ---  | ---      | ---  | ---      | ---      | ---        | ---   | ---   |
| **PointNet MLS**   |90.83%|75.58%    |64.14%|94.95%    |83.12%    |81.19%      |57.10% |23.31% |
| **PointNet HMLS**  |62.20%|70.31%    |0.00% |94.95%    |63.91%    |78.56%      |61.75% |51.69% |
| **PointNet H&MLS** |85.21%|73.00%    |30.35%|96.16%    |82.89%    |84.65%      |50.54% |45.05% |           

## Point Cloud attributes
### MLS point clouds
- XYZ
- Number of Retuns
- Return number
- GPS Time
- Intensity
- Classification

### HMLS point clouds
- XYZ
- Classification

## Classes
- Road (label 0)
- Sidewlak (label 1)
- Curb (label 2)
- Building (label 3)
- Vehicles (label 4)
- Vegetation (label 5)
- Poles (Sings, Traffic lights and Street lights) (label 6)
- Others (label 7)

## Download
Dataset can be download at [OneDrive](https://universidadevigo-my.sharepoint.com/:f:/g/personal/silvgonzalez_uvigo_gal/Em0OZC-FmxtBgrXdZgxGrewBdVgkexzcJ-SDFIYJSMRK5A?e=mZMWnZ)

## Citation
Silvia María González-Collazo, Jesús Balado, Iván Garrido, Javier Grandío, Rabia Rashdi, Elisavet Tsiranidou, Pablo del Río-Barral, Erik Rúa, Iván Puente, Henrique Lorenzo,
Santiago urban dataset SUD: Combination of Handheld and Mobile Laser Scanning point clouds,
Expert Systems with Applications,
Volume 238, Part B,
2024,
121842,
ISSN 0957-4174,
https://doi.org/10.1016/j.eswa.2023.121842.

## Avknowledgements
This research was funded by the Xunta de Galicia, grant numbers ED481B-2019-061 and ED431C 2020/01, and by the Ministerio de Ciencia, Innovación y Universidades -Gobierno de España-, grant number PID2019-105221RB-C43/AEI/10.13039/501100011033. This paper was carried out in the framework of the InfraROB project (Maintaining integrity, performance and safety of the road infrastructure through autonomous robotized solutions and modularization), which has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement no. 955337. It reflects only the authors’ views. Neither the European Climate, Infrastructure, and Environment Executive Agency (CINEA) nor the European Commission is in any way responsible for any use that may be made of the information it contains. Authors also would like to thank to CESGA for the use of their servers. Funding for open access charge: Universidade de Vigo/CISUG.
