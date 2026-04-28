# HBN Dataset

\# Handwritten Babylonian Numerals (HBN) Dataset



\## 📌 Overview



The \*\*Handwritten Babylonian Numerals (HBN) Dataset\*\* is a large-scale benchmark dataset designed for research in \*\*computer vision, pattern recognition, and computational archaeology\*\*. It focuses on the recognition of ancient Babylonian numerals using modern machine learning techniques.



This dataset bridges historical numeral systems with artificial intelligence, enabling the study of structural patterns in one of the earliest known mathematical notations.



\---
## 🔗 Dataset Repository
Access the dataset here:  
[HBN Dataset on GitHub](https://github.com/drloay40/HBN-Dataset)

\## 📊 Dataset Statistics



\* \*\*Total images:\*\* 14,000

\* \*\*Number of classes:\*\* 14

\* \*\*Classes:\*\* 1–9, 10, 20, 30, 40, 50

\* \*\*Participants:\*\* 100

\* \*\*Samples per participant:\*\* 140

\* \*\*Image format:\*\* PNG/JPG

\* \*\*Image type:\*\* Binary (1-bit) or Grayscale

\* \*\*Typical resolution:\*\* \~100×100 (raw), standardized to 128×128 (processed)



\---



\## 🧠 Dataset Description



The dataset is based on the \*\*Babylonian sexagesimal (base-60) numeral system\*\*, which uses combinations of wedge-shaped symbols:



\* Vertical wedge → units (1–9)

\* Corner wedge → tens (10, 20, ..., 50)



Each numeral is constructed using combinations of these base symbols.



\---



\## 🏗️ Data Collection Process



\* Participants reproduced numerals on structured forms

\* Each participant wrote \*\*14 numerals × 10 repetitions\*\*

\* Forms were scanned at \*\*300 dpi\*\*

\* Images were segmented into individual samples



\---



\## ⚙️ Preprocessing Pipeline



The dataset includes preprocessing steps such as:



\* Grayscale conversion

\* Noise reduction (Gaussian filtering)

\* Adaptive thresholding

\* Normalization

\* Resizing to \*\*128×128 pixels\*\*

\* Centering and padding



Optional:



\* Edge detection (Canny)



\---



\## 🔄 Data Augmentation



To improve robustness, the dataset supports:



\* Rotation

\* Scaling

\* Translation



\---



\## 📁 Dataset Structure



```bash

HBN-Dataset/

└── data/

&#x20;   ├── 01/

&#x20;   ├── 02/

&#x20;   ├── ...

&#x20;   ├── 09/

&#x20;   ├── 10/

&#x20;   ├── 20/

&#x20;   ├── 30/

&#x20;   ├── 40/

&#x20;   └── 50/

```



Each folder represents one class label.



\---



\## 🏷️ Naming Convention



Files follow the format:



```

userID\_numeralValue\_index

```



Example:



```

U01\_10\_03.png

```



\---



\## 🤖 Benchmark Performance



The dataset was validated using a CNN-based model (\*\*StructFusionNet\*\*):



\* \*\*Accuracy:\*\* 98.33%

\* \*\*Precision:\*\* 98.21%

\* \*\*Recall:\*\* 98.28%



This confirms the dataset’s suitability for deep learning applications.



\---



\## 🎯 Applications



\* Handwritten numeral recognition

\* Historical script analysis

\* Writer identification

\* Pattern recognition research

\* Deep learning benchmarking



\---



\## 📄 Paper



If you use this dataset, please cite:



\*\*"Handwritten Babylonian Numerals (HBN) Dataset: A Benchmark for Structural Feature Analysis and Deep Learning-Based Recognition"\*\*



(Include your full citation here)



\---



\## ⚙️ Usage



```bash

git clone https://github.com/your-username/HBN-Dataset.git

```



Example (Python):



```python

from tensorflow.keras.preprocessing.image import ImageDataGenerator



datagen = ImageDataGenerator(rescale=1./255)



dataset = datagen.flow\_from\_directory(

&#x20;   'data/',

&#x20;   target\_size=(128,128),

&#x20;   color\_mode='grayscale',

&#x20;   class\_mode='categorical'

)

```



\---



\## 📜 License



This dataset is released under the \*\*Creative Commons Attribution 4.0 International (CC BY 4.0)\*\* license.



You are free to use, share, and adapt the data with proper attribution.



\---



\## ⚖️ Ethics Statement



\* All participants provided informed consent

\* No personal or identifying information is included

\* Dataset is intended for academic and research use



\---



\## 👤 Authors



\* Loay Alzubaidi
\* Jaber Jemai
\* Ashraf Alkaraki 
\* Abdulla Aljuaidi
\* Ali Alghailani



\---



\## 🙌 Acknowledgments



Supported by \*\*Higher Colleges of Technology (HCT), UAE\*\*.



Special thanks to all participants and contributors involved in data collection and processing.



\---



