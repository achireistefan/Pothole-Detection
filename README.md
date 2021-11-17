# Pothole-Detection

The presented dataset is an aggregation of the below presented datasets, resulting a total number of 1490 annotated images with two unique labels: pothole and drain.

Dataset 1: SoV Pothole Detection Dataset is the dataset recorded during this project. It is acquired using a ZED 2 stereo camera mounted on the forehead and chest. From the four sequences, were extracted a total of 447 images with annotated potholes and drains. We extracted the left frame, right frame and depth map for each image.

Dataset 2: Potholes Detection Dataset [1] consists of 665 annotated potholes. The dataset was created and shared by Atikur Rahman Chitholian as part of his thesis. The original dataset did not contain a validation set, later was re-shuffled into a 70-20-10% train-validation-test split. The dataset is provided in a wide variety of formats for the most common models, YOLO included.

Dataset 3: MIIA Pothole Image Dataset [2] was proposed in 2019 by the Machine Intelligence Institute of Africa for an image classification challenge. The goal is to create a machine learning model that can accurately predict the likelihood that an image contains or not potholes. The dataset contains 5676 images of streets in South Africa with and without potholes. The data have been split into 4026 images for training and 1650 for testing. The provided classification labels (1-potholes, 0-no potholes) could not be used for the purpose of this paper, therefore a selection of the dataset was manually annotated with bounding boxes for each pothole.

Dataset 4: Another considered dataset [3] is constructed of 90 pothole images without any annotation. It was manually annotated and split into train-val-test subsets.

Train-val-test split

Finally, the obtained dataset was randomly split by a 70:20:10 train-val-test ratio. For better results, the train-val subset (1341 images) was augmented applying the following six operations:

• vertical flip; <br />
• horizontal flip;

• vertical-horizontal flip;

• 90o rotation;

• average blurring;

• raise the hue value.

We provide pascal voc and yolo annotation for the augmented pothole detection dataset.
When using this dataset in your research, we will be happy if you cite us:
@INPROCEEDINGS{Achirei2021ICCP,
  author = {Stefan-Daniel Achirei and Ioana-Ariana Opariuc and Otilia Zvoristeanu and Simona Caraiman and Vasile-Ion Manta},
  title = {Pothole Detection for Visually Impaired Assistance},
  booktitle = {International Conference on Intelligent Computer Communication and Processing (ICCP)},
  year = {2021}
}


[1] Atikur Rahman Chitholian, Pothole Dataset, available online: https://github.com/chitholian/Potholes-Detection OR https://public.roboflow.ai/object-detection/pothole

[2] Machine Intelligence Institute of Africa, MIIA Pothole Image Classification Challenge, available online: https://zindi.africa/competitions/miia-pothole-image-classification-challenge

[3] Pothole Detection Dataset, online https://people.etf.unsa.ba/~aakagic/pothole_detection/
