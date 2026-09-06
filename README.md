Handwritten Babylonian Numerals (HBN) Dataset
The Handwritten Babylonian Numerals (HBN) Dataset is an open dataset
for handwritten Babylonian numeral recognition, image classification,
structural feature analysis, historical document processing, and
computational research on ancient scripts.
The dataset contains 14,000 original handwritten numeral images
collected from 100 participants. It covers 14 numeral classes:
1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 20, 30, 40, and 50
Each participant reproduced every class 10 times on a structured
paper collection form. This gives:
14 classes × 10 repetitions = 140 samples per participant
100 participants × 140 samples = 14,000 original images
100 participants × 10 repetitions = 1,000 original images per
class
Dataset Characteristics
Property                                Description
---
Numeral system                          Babylonian sexagesimal (base-60)
Number of classes                       14
Target values                           1--9, 10, 20, 30, 40, 50
Participants                            100
Repetitions per class per participant   10
Samples per participant                 140
Original samples per class              1,000
Total original images                   14,000
Scanning resolution                     300 dpi
Final image representation              Grayscale
Final image size                        128 × 128 pixels
Augmented images included               No
License                                 CC BY 4.0
Data Collection
HBN was created in response to the limited availability of suitable
image resources for handwritten Babylonian numeral recognition.
A structured paper-based collection form was designed with predefined
writing regions for the 14 target numeral classes. Participants were
shown the target numeral forms and reproduced each class ten times in
its designated region.
The predefined form layout provides a known relationship between each
writing region and its numeral class. This supports systematic image
extraction and position-based labeling without requiring independent
visual class annotation for every sample.
Completed forms were digitized at 300 dpi.
Segmentation and Labeling
Each completed form contains 140 handwritten samples. Individual
samples were extracted using predetermined row and column coordinate
boundaries corresponding to the structured writing regions.
The processing sequence was:
Load and verify the scanned collection form.
Locate writing regions using predetermined coordinates.
Extract each individual numeral region.
Assign the class label from the known position on the form.
Associate the image with its participant, numeral class, and
repetition number.
Store the processed image in the corresponding class organization.
This procedure yields 14,000 original labeled images from 100
completed forms.
Image Preprocessing
The released HBN images were standardized through the following
procedure:
Collection-form frame removal --- the printed square boundary
surrounding each writing region was removed so that the template
frame did not become part of the numeral representation.
Grayscale conversion --- extracted images were represented as
single-channel grayscale images.
Numeral-region isolation and cropping --- unnecessary
surrounding background was reduced while preserving the complete
handwritten symbol.
Image standardization --- images were resized to 128 × 128
pixels.
Organization --- images were stored according to their class and
identifying information.
No data augmentation is included in the 14,000-image HBN dataset
described here.
Dataset Organization
The dataset is organized by numeral class. A participant/class/sample
naming structure can be used to preserve traceability:
`participantID_numeralValue_sampleIndex`
Example:
`U023_20_07`
This identifies the seventh handwritten sample of numeral 20 associated
with participant 23.
Participant identifiers are anonymized and are intended for dataset
organization and writer-independent experimental protocols.
Suggested Uses
HBN can support research and teaching in:
Handwritten Babylonian numeral recognition
Image classification
Structural feature analysis
Pattern recognition
Writer-independent recognition
Representation learning and transfer learning
Historical document analysis
Digital humanities
Computational archaeology
Ancient-script analysis
Scope
HBN contains handwritten numeral samples collected on structured paper
forms. It does not represent authentic clay-tablet imagery, damaged
archaeological documents, or complete multi-symbol cuneiform texts.
Models trained on HBN should therefore be evaluated with appropriate
domain-specific data before being assumed to generalize to
archaeological tablet images.
Authors
Loay Alzubaidi
Jaber Jemai
Ashraf Alkaraki
Rajesh Thomas
Faculty of Computing and Information Systems  
Higher Colleges of Technology, United Arab Emirates
Corresponding author: Loay Alzubaidi --- lalzubaidi@hct.ac.ae
Related Publications
The HBN handwritten numeral collection has supported research on
Babylonian numeral recognition, including:
L. Alzubaidi, I. Al-Qudah, and K. E. Bouazza, "Deep Learning
Approaches to Babylonian Numeral Recognition: A CNN--SVM Hybrid
Model," 2024 IEEE International Conference on Computing (ICOCO),
Kuala Lumpur, Malaysia, 12--14 Dec. 2024, pp. 140--145. DOI:
10.1109/ICOCO62848.2024.10928249.
L. Alzubaidi, A. Alnahdi, A. Ahmed, N. Waheed, and A. El Hassan,
"StructFusionNet: Structural Feature Fusion in CNNs for Handwritten
Babylonian Numeral Recognition," Applied Computational Intelligence
and Soft Computing, 2026, Article ID 4724541. DOI:
10.1155/acis/4724541.
L. Alzubaidi, K. E. Bouazza, and I. Al-Qudah, "A Hybrid Deep
Learning Framework for Multi-Symbol Recognition and Positional
Decoding of Handwritten Babylonian Numerals," Algorithms, vol. 19,
no. 4, article 322, 2026. DOI: 10.3390/a19040322.
The multi-symbol composite images created for the third study are
downstream derived research data and are not part of the original
14,000-image HBN collection.
Citation
If you use HBN in research, please cite the associated HBN data article
once its final bibliographic details are available. Until then, please
cite this repository and the relevant related publication(s).
Suggested repository citation:
> Alzubaidi, L., Jemai, J., Alkaraki, A., & Thomas, R. *Handwritten
> Babylonian Numerals (HBN) Dataset*. Higher Colleges of Technology,
> United Arab Emirates. GitHub repository.
License
The HBN Dataset is released under the Creative Commons Attribution 4.0
International (CC BY 4.0) license.
License information: https://creativecommons.org/licenses/by/4.0/
Under CC BY 4.0, users may share and adapt the material, including for
commercial purposes, provided appropriate attribution is given and the
other license requirements are followed.
Repository
HBN Dataset: https://github.com/drloay40/HBN-Dataset
Contact
For questions concerning the dataset:
Loay Alzubaidi  
Faculty of Computing and Information Systems  
Higher Colleges of Technology, United Arab Emirates  
Email: lalzubaidi@hct.ac.ae
