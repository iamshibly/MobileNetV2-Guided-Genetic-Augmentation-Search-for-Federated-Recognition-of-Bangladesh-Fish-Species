# MobileNetV2-Guided Genetic Augmentation Search for Federated Recognition of Bangladeshi Freshwater Fish Species

<div align="center">

# Dataset and Nutrition CSV

## **[Access the Dataset and Nutrition CSV](PASTE_YOUR_GOOGLE_DRIVE_LINK_HERE)**

### **The Google Drive folder contains the freshwater fish image dataset and the per-100g nutrition metadata CSV file.**

**Available through the Drive link:**

**Raw fish image dataset**  
**Species-wise image folders**  
**Per-100g nutrition values CSV file**  
**Dataset files required for training and evaluation**

</div>

---

## Project Overview

This repository contains a lightweight deep learning and federated learning framework for recognizing Bangladeshi freshwater fish species using a **MobileNetV2-based recognition model**.

The project focuses on freshwater fish species classification in a simulated federated learning environment. It also supports nutrition-aware analysis through a structured CSV file containing **per-100g nutritional values** for each fish class.

The repository is organized into three main experimental parts:

- **Proposed Method**
- **Ablation Studies**
- **Baseline Comparison**

The main goal is to evaluate whether a MobileNetV2-based lightweight framework can provide a practical and robust solution for freshwater fish species recognition using Bangladesh-focused fish image data.

---

## Key Features

- MobileNetV2-based lightweight fish recognition framework
- Federated learning-based recognition setting
- Client-wise simulated training setup
- Ablation studies for component-level analysis
- Baseline comparison with alternative deep learning backbones
- Dataset support for 23 Bangladeshi freshwater fish species
- Per-class nutrition metadata using a per-100g nutrition CSV file
- Suitable for image classification, food recognition, and nutrition-aware AI research

---

## Repository Structure

```text
MobileNetV2-Guided-Genetic-Augmentation-Search-for-Federated-Recognition-of-Bangladeshi-Freshwater-Fish-Species/
│
├── Proposed Method/
│   └── Files related to the proposed MobileNetV2-guided federated recognition framework
│
├── Ablation Studies/
│   └── Files related to ablation experiments
│
├── Baseline Comparison/
│   └── Files related to baseline backbone comparison experiments
│
└── README.md
```

---

## Dataset Access

The dataset and nutrition CSV are available through the Google Drive link shown at the top of this README.

After downloading the dataset, the expected structure is:

```text
Fish Dataset/
│
├── Fish Dataset Raw/
│   ├── Bacha/
│   ├── Baim/
│   ├── Bele/
│   ├── Chanda/
│   ├── Cheng/
│   ├── Dairka/
│   ├── Dhaira/
│   ├── Dhyala-pithali/
│   ├── Fasa/
│   ├── Goti/
│   ├── Guchi/
│   ├── Itha/
│   ├── Jiyol/
│   ├── Kakila/
│   ├── Khori/
│   ├── Koi/
│   ├── Mohola/
│   ├── Pabda/
│   ├── Paloa Tengra/
│   ├── Piyali/
│   ├── Puthi/
│   ├── Rewa/
│   └── Veda/
│
└── nutrition_per_100g.csv
```

---

## Dataset Summary

The dataset contains freshwater fish images from Bangladesh and a nutrition metadata CSV file.

| Dataset Component | Count / Description |
|---|---:|
| Fish species/classes | 23 |
| Raw images | 5,520 |
| Nutrition metadata | Per 100g edible portion |
| Main data types | Image + CSV |

The image dataset is organized into species-wise folders, making it suitable for supervised image classification and federated learning experiments.

---

## Fish Species Included

The dataset contains the following 23 fish categories:

| No. | Fish Category |
|---:|---|
| 1 | Bacha |
| 2 | Baim |
| 3 | Bele |
| 4 | Chanda |
| 5 | Cheng |
| 6 | Dairka |
| 7 | Dhaira |
| 8 | Dhyala / Pithali |
| 9 | Fasa |
| 10 | Goti |
| 11 | Guchi |
| 12 | Itha |
| 13 | Jiyol |
| 14 | Kakila |
| 15 | Khori |
| 16 | Koi |
| 17 | Mohola |
| 18 | Pabda |
| 19 | Paloa Tengra |
| 20 | Piyali |
| 21 | Puthi |
| 22 | Rewa |
| 23 | Veda |

---

## Nutrition CSV

The Drive folder includes a CSV file containing species-level nutritional values per 100g edible portion.

The nutrition CSV can be used for:

- Nutrition-aware fish recognition
- Class-wise nutrition analysis
- Food image understanding
- Dietary decision-support systems
- Multimodal image and tabular learning
- Fish recommendation based on nutritional properties

Possible nutrition fields include:

| Field Type | Example Fields |
|---|---|
| Identity | Local name, scientific name |
| Energy | Energy value |
| Macronutrients | Protein, fat |
| Vitamins | Vitamin A, Vitamin B12 |
| Minerals | Calcium, phosphorus, potassium, sodium, iron |
| Fatty acids | Omega-3, Omega-6 |

---

## Proposed Method

The proposed method uses a **MobileNetV2-based framework** for lightweight freshwater fish recognition.

The method combines:

1. Fish image input
2. Client-wise data partitioning
3. Client-side model training
4. MobileNetV2-based feature learning
5. Federated aggregation
6. Global model evaluation
7. Final fish species prediction

General workflow:

```text
Fish Images
    ↓
Client-wise Data Partitioning
    ↓
Client-side Training
    ↓
MobileNetV2 Feature Learning
    ↓
Federated Aggregation
    ↓
Global Model Evaluation
    ↓
Fish Species Prediction
```

---

## Federated Learning Setting

This project uses a simulated federated learning setup.

Instead of training on one centralized dataset only, the dataset is divided into client partitions. Each client trains locally, and the global model is updated using federated aggregation.

This setup is useful for future real-world cases where fish image data may come from different sources, such as:

- Local markets
- Mobile devices
- Regional data collection centers
- Fisheries offices
- Research institutions

Federated learning is useful when data is distributed and centralized sharing is not ideal.

---

## Proposed Experimental Setting

The proposed setting includes:

- MobileNetV2-based local client training
- Federated aggregation across simulated clients
- Global model evaluation using held-out test data
- Species-wise classification performance analysis

This setup evaluates whether a lightweight MobileNetV2-based model can perform effectively for Bangladeshi freshwater fish recognition under a federated learning environment.

---

## Ablation Studies

Ablation studies are included to evaluate how different components affect the final performance.

| Group | Setting |
|---|---|
| Proposed | MobileNetV2-based federated recognition framework |
| Ablation 1 | No client preprocessing |
| Ablation 2 | Client preprocessing included |
| Ablation 3 | Alternative client-side setting |
| Ablation 4 | Training and testing with the same client-side setting |
| Ablation 5 | Model setting without adapter regularization |

These experiments help analyze how client-side settings and model components influence recognition performance.

---

## Baseline Comparison

The baseline comparison evaluates whether the proposed MobileNetV2-based framework remains competitive against other backbone models.

| Baseline | Backbone |
|---|---|
| Backbone baseline 1 | DenseNet121 |
| Backbone baseline 2 | MobileNet with alpha = 0.75 |
| Backbone baseline 3 | NASNetMobile |
| Backbone baseline 4 | Xception |

---

## Evaluation Metrics

The experiments can be evaluated using standard multi-class classification metrics:

- Accuracy
- Balanced accuracy
- Precision
- Recall
- Macro-F1 score
- Weighted-F1 score
- Confusion matrix
- Class-wise F1 score
- Client-wise performance
- Fold-wise performance

Because the dataset contains class imbalance, macro-F1 and balanced accuracy are especially useful along with overall accuracy.

---

## Requirements

Recommended Python environment:

```text
Python 3.8+
NumPy
Pandas
Scikit-learn
Matplotlib
OpenCV
Pillow
Tqdm
TensorFlow / Keras or PyTorch
```

Install common dependencies:

```bash
pip install numpy pandas scikit-learn matplotlib opencv-python pillow tqdm
```

If using TensorFlow:

```bash
pip install tensorflow
```

If using PyTorch:

```bash
pip install torch torchvision
```

---

## How to Use

### 1. Clone the Repository

```bash
git clone https://github.com/iamshibly/MobileNetV2-Guided-Genetic-Augmentation-Search-for-Federated-Recognition-of-Bangladeshi-Freshwater-Fish-Species.git
cd MobileNetV2-Guided-Genetic-Augmentation-Search-for-Federated-Recognition-of-Bangladeshi-Freshwater-Fish-Species
```

### 2. Download the Dataset

Download the image dataset and nutrition CSV from the Drive link at the top of this README.

Place the dataset in the project root:

```text
project-root/
│
├── Fish Dataset/
│   ├── Fish Dataset Raw/
│   └── nutrition_per_100g.csv
│
├── Proposed Method/
├── Ablation Studies/
├── Baseline Comparison/
└── README.md
```

### 3. Run Proposed Method

```bash
cd "Proposed Method"
python main.py
```

### 4. Run Ablation Studies

```bash
cd "Ablation Studies"
python main.py
```

### 5. Run Baseline Comparison

```bash
cd "Baseline Comparison"
python main.py
```

> Note: If the script names are different inside each folder, replace `main.py` with the correct file name.

---

## Expected Outputs

Depending on the scripts provided in each folder, the experiment outputs may include:

- Training accuracy curves
- Validation accuracy curves
- Training loss curves
- Validation loss curves
- Confusion matrices
- Classification reports
- Client-wise result tables
- Fold-wise result tables
- Ablation result tables
- Backbone comparison result tables

---

## Possible Applications

This repository can support:

- Bangladeshi freshwater fish species recognition
- Lightweight food recognition systems
- Mobile fish recognition
- Federated image classification research
- Nutrition-aware computer vision
- Fish market decision-support systems
- Fisheries data analysis
- Image and nutrition multimodal learning
- Educational and academic research on local fish species

---

## Usage Note

Please download the dataset and nutrition CSV from the Drive link provided at the top of this README before running the code.

Make sure the image folders and nutrition CSV file are placed in the correct directory before training or evaluation.

---

## License

This repository is intended for academic and research use.

Please check the dataset folder or repository license before using the dataset or code for commercial purposes.

---

## Acknowledgement

This project supports research on freshwater fish recognition, lightweight deep learning, federated learning, and nutrition-aware computer vision for Bangladesh-focused fish species analysis.
