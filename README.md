# Blood Cell Classification Project

## Table of Contents
1. [Introduction](#introduction)
2. [Datasets](#datasets)
    * [BCCD Dataset](#bccd-dataset)
    * [Complete Blood Count (CBC) Dataset](#complete-blood-count-cbc-dataset)
    * [PBC_dataset_Normal_DIB](#pbc_dataset_normal_dib)
3. [Project Structure](#project-structure)
4. [Setup and Installation](#setup-and-installation)
5. [Usage](#usage)
    * [Data Preparation](#data-preparation)
    * [Model Training](#model-training)
    * [Model Evaluation](#model-evaluation)
6. [Acknowledgements](#acknowledgements)
7. [License](#license)
8. [Contact](#contact)

## Introduction
This project focuses on the classification of blood cells using a convolutional 
neural network (CNN) model implemented with TensorFlow. The datasets used in 
this project are BCCD Dataset, Complete Blood Count (CBC) Dataset, and 
PBC_dataset_Normal_DIB,

## Datasets
### BCCD Dataset
BCCD Dataset is a small-scale dataset for blood cells detection. The dataset includes
three types of lables: RBC (Red Blood Cell), WBC (White Blood Cell), and Platelets.

#### Overview
* **Image type**: JPEG
* **Image size**: 640x480
* **Annotations**: VOC format XML files

For more details, see For more details, see the [BCCD Dataset README](https://github.com/Shenggan/BCCD_Dataset/blob/master/README.md).

### Complete Blood Count (CBC) Dataset
The CBC dataset contains 360 blood smear images along with their annotation files, 
split into training, testing, and validation sets. It includes images annotated for
RBC, WBC, and Platelets.

#### Overview
* **Image type**: JPEG
* **Image size**: 640x480
* **Annotations**: VOC format XML files

For more details, see the [CBC Dataset README](https://github.com/MahmudulAlam/Complete-Blood-Cell-Count-Dataset/blob/master/README.md).

### PBC_dataset_Normal_DIB
This dataset contains 17,092 images of individual normal cells, organized into eight groups:
* Eosinophils
* Lymphocytes
* Monocytes
* Neutrophils
* Basophils
* Platelets
* Immature granulocytes
* Erythroblasts

The images were acquired using the analyzer CellaVision DM96 in the Core Laboratory
at the Hospital Clinic of Barcelona and annotated by expert clinical pathologists.

#### Overview
* **Image type**: JPEG
* **Image size**: 360x363
* **Annotations**: in file names

For more details, see the [PBC_dataset_Normal_DIB on Mendeley Data](https://data.mendeley.com/datasets/snkd93bnjr/1).
## Project Structure
```
.
├── BCCD_dataset
│   ├── BCCD
│   │    ├── Annotations
│   │    ├── ImageSets
│   │    └── JPEGImages
│   ├── dataset
│   │   └── mxnet
│   │       ├── prepro.py
│   │       └── test.py
│   ├── scripts
│   │   ├── split.py
│   │   └── visualize.py
│   ├── example.jpg
│   ├── export.py
│   ├── LICENCE
│   ├── plot.py
│   ├── README.md
│   └── test.csv
├── Complete-Blood-Cell-Count-Dataset
│   ├── Testing
│   │   ├── Annotations
│   │   └── Images
│   ├── Training
│   │   ├── Annotations
│   │   └── Images
│   ├── Validation
│   │   ├── Annotations
│   │   └── Images
│   ├── _config.yml
│   ├── LICENSE
│   └── README.md
├── Model
│   ├── my_model
│   │   └── assets
│   ├── variables
│   │   ├── variables.data-00000-of-00001
│   │   └── variables.index
│   ├── fingerprint.pb
│   ├── keras_metadata.pb
│   └── saved_model.pb
├── PBC_dataset_Normal_DIB
│   ├── basophil
│   ├── eosinophil
│   ├── erythroblast
│   ├── ig
│   ├── lymphocyte
│   ├── monocyte
│   ├── neutrophil
│   └── platelet
├── unified_dataset
│   └── Images
├── .gitignore
├── LICENSE
├── Blood_Cell_Classification.ipynb
├── requirements.txt
└── README.md
```
## Setup and Installation
1. Clone the repository:
```bash
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
```
2. Create and activate a virtual environment:
```bash
python3.8 -m venv venv
source venv/bin/activate
```
3. Install the required packages:
```bash
pip install -r requirements.txt
```
## Usage
### Data Preparation
Data preparation scripts are provided in the `Blood_Cell_Classification.ipynb` notebook.
### Model Training
The model training script is provided in the `Blood_Cell_Classification.ipynb` notebook.
### Model Evaluation
The model evaluation script is provided in the `Blood_Cell_Classification.ipynb` notebook.
## Acknowledgements
* BCCD_Dataset: Thanks to [Shenggan](https://github.com/Shenggan) and [Nicolas Chen](https://github.com/nicolaschen1) for providing the BCCD Dataset.
* Complete Blood Count (CBC) Dataset: Thanks to [MahmudulAlam](https://github.com/MahmudulAlam/Complete-Blood-Cell-Count-Dataset/commits?author=MahmudulAlam) for providing the CBC Dataset.
* PBC_dataset_Normal_DIB: Thanks to the authors of the [PBC_dataset_Normal_DIB](https://data.mendeley.com/datasets/snkd93bnjr/1) dataset.
## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
**Note**: The datasets used in this project have their own licenses. Please refer to the original sources for more information.
## Contact 
If you have any questions or suggestions, please feel free to contact me at [bv2340@columbia.edu](bv2340@columbia.edu).

