# Mesoscale-Eddy-Dataset

We constructed a benchmark dataset for **mesoscale eddy detection** that integrates multimodal data. Specifically, the dataset combines **sea level anomaly (SLA)**, **sea surface height (SSH)**, **sea surface temperature (SST)**, and **chlorophyll-a (CHL) concentration**, thereby providing complementary information for eddy detection. Overall, the dataset comprises **341,500** mesoscale eddies, including **173,651** anticyclone eddies and **167,849** cyclone eddies.

## Data Specifications

* **Spatiotemporal Resolution**: The multimodal data have a spatial resolution of **0.25° × 0.25°** and a daily temporal resolution.

* **Temporal Coverage**: Each dataset covers **2,000** consecutive days.

* **Dimensions**: The original data dimensions of 129 × 129 pixels have been upsampled by a factor of five to a final resolution of **645 × 645** pixels.

## Study Areas

* The Area-1 covers the region from **5°N** to **37°N** and **104°E** to **136°E**. This subset is further divided into two subregions: Area-2 and Area-3.

* The Area-4 covers the region from **19°N** to **51°N** and **47°W** to **79°W**. 

Each dataset contains **2,000** images in total. Among them, the first **1,635** images are used for training, while the remaining **365** images are reserved for testing. Detailed information is provided in the table below.

| Ocean     | Spatial coverage      | Temporal coverage     |
| ---       | ---                   | ---                   |
| Area-1    | 5°-37°N, 104°-136°E   | 2016.8.19-2022.2.9    |
| Area-2    | 5°-23°N, 105°-121°E   | 2016.8.19-2022.2.9    |
| Area-3    | 23°-34°N, 117°-131°E  | 2016.8.19-2022.2.9    |
| Area-4    | 19°-51°N, 47°-79°W    | 2017.12.16-2023.6.7   |

The instance sizes for these datasets are presented in the table below.

| Ocean     | Train          |            | Test           |            | Total          |            | 
| ---       | ---            | ---        | ---            | ---        | ---            | ---        |
|           | Anticyclone    | Cyclone    | Anticyclone    | Cyclone    | Anticyclone    | Cyclone    |
| Area-1    | 80,190         | 76,747     | 13,060         | 12,681     | 93,250         | 89,428     |
| Area-2    | 22,840         | 21,521     | 3,715          | 3,728      | 26,555         | 24,863     |
| Area-3	  | 20,734         | 18,599     | 3,638          | 3,342      | 24,372         | 21,941     |
| Area-4    | 66,670         | 64,444     | 13,731         | 13,977     | 80,401         | 78,421     |

# Samples

Here are two examples of raw unannotated and annotated data.

### Area-1

![](./china_sea.png)

### Area-4

![](./atlantic.png)

# Multi-Task Applications

* The dataset can be used for multimodal mesoscale eddy object detection tasks.
* Based on the area ratio of the images, small objects account for more than **2/3** (**105,056** objects) of this dataset, making it suitable for small object detection.
* cross-domain object detection

<br>

> ⚠ **Note:** The dataset will be further refined and made publicly available to support future research efforts.

# License

lease notice that this dataset is made available for academic research purposes only, the copyright belongs to the original owners.
