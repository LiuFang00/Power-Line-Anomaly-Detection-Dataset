# TransLine_Image_Dataset
This dataset is mainly used to support the research on anomaly power line detection. 

**If you would like to use this dataset, please help to cite our papers shown below:**

1. \[TPCI\] Fang Liu, Wei Zhang (corresponding author), Indriyati Atmosukarto et al. “TransLine: Transfer Learning for Accurate and Explainable Power Line Anomaly Detection with Insufficient Data.” CCF Transactions on Pervasive Computing and Interaction (TPCI), pp. 1-14. May, 2023. [PDF](https://drive.google.com/file/d/1xlFw19fNJ2rvbx-m56LS9C1YeIn-gF8I/view?pli=1)
2. \[ICC '22\] Fang Liu, Teck Wei Low, Wei Zhang (corresponding author) et al. “TransLine: Transfer Learning for Accurate Power Line Anomaly Detection with Insufficient Data.” IEEE International Conference on Communications (ICC), pp. 5543-5548. IEEE. Seoul, South Korea. May 16–20, 2022.

### Problem
Data is a necessity for power line anomaly detection. With the technology advancements in the past decades, various imaging terminals are available nowadays, e.g., electric vehicles, UAVs, and perhaps even Spot by Boston Dynamics in the near future. However, a problem still exists for power line data. While it is not difficult to get data, data is often highly biased and imbalanced. It is well-known that an anomaly rarely occurs.

### Dataset Introduction
Here, we use the Internet as a portal with key avenues such as GitHub, data websites, and Google Images. The first two are academia-centric, where normal power line data can be collected but anomaly data is limited. We thus further consider the general-purpose Google Images, which allows us to search by keywords, e.g., broken and downed power lines. Such targeted searches enable us to get anomaly data and deliver a non-biased and balanced dataset. Each image in the dataset is manually annotated as either normal or abnormal by a researcher and audited by a different researcher. Images are also carefully selected such that there is only one image from the same scene, and similar ones, e.g., with slightly different angles or brightness, are excluded. Processed dataset for power line images labeled with two classes 'broken' and 'normal'.

### Normal Power Lines
The normal images are collected and integrated from the three sources. A total of 405 normal power line images were collected.
1. The first one is a GitHub data repository [https://github.com/r3ab/ttpla_dataset], which includes aerial images of power lines and transmission towers. This dataset is mainly used for object detection and segmentation applications, so abnormal images are not necessary and all the images are normal. From the set of images, a subset of 360 suitable images were extracted and included in our dataset for normal power lines.
2. The second one is a website called Mendeley Data, with a power line dataset for infrared and visible light images. We select 10 images solely for power lines and include them in our dataset. The above two sources are highly specialized and the images are all of high quality.
3. The third one is Google Image. To further enrich our dataset with images of low and median quality, we collected 35 additional images from Google Images.

### Broken Power Lines
Anomaly data is collected from Google Images through keyword search and manual labeling. We consider two types of anomalies. One is for broken power lines where damages can be visually seen in the images. The other is for downed power lines, where the line is not broken but impacted by some objects like fallen trees. A total of 120 abnormal images were collected consisting of 74 broken power line images and 46 downed power lines images.
