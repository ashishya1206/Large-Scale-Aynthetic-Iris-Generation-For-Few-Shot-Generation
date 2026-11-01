Large-Scale Synthetic Iris Generation for Few-Shot Recognition
Research Project Repository
1. Project Overview
This repository contains the materials for the research project Large-Scale Synthetic Iris Generation for Few-Shot Recognition.
The project investigates the generation of synthetic iris images using deep learning, with the objective of supporting iris recognition under few-shot learning conditions.
The research workflow covers iris dataset exploration, segmentation, normalization, image enhancement, quality assessment, few-shot dataset construction, identity representation learning, diffusion-based synthetic image generation, identity verification, diversity analysis, recognition evaluation, and statistical analysis.
The repository is organized to support reproducibility, collaborative development, and evaluation of the research work.
Project status: Research implementation and experimentation are in progress. Final results and conclusions will be added after experimental validation.
2. Research Objectives
The main objectives are:
Explore and preprocess available iris image datasets.
Perform iris segmentation and normalization.
Assess and improve iris image quality.
Construct few-shot training and evaluation datasets.
Develop a deep learning-based synthetic iris generation pipeline.
Evaluate the identity consistency and diversity of generated iris images.
Investigate whether synthetic data improves few-shot iris recognition.
Compare performance across datasets and experimental settings.
Perform ablation studies and statistical significance testing.
3. Repository Structure
LargeScale_Synthetic_Iris_Generation/
│
├── datasets/
│
├── pretrained_models/
│
├── generated_images/
│   └── README.md
│
├── results/
│
├── notebooks/
│   ├── 01_Dataset_Exploration.ipynb
│   ├── 02_Iris_Segmentation.ipynb
│   ├── 03_Iris_Normalization.ipynb
│   ├── 04_Image_Enhancement.ipynb
│   ├── 05_Image_Quality_Assessment.ipynb
│   ├── 06_FewShot_Dataset_Creation.ipynb
│   ├── 07_Baseline_Recognition.ipynb
│   ├── 08_Identity_Latent_Space.ipynb
│   ├── 09_Diffusion_Model_Training.ipynb
│   ├── 10_Synthetic_Image_Generation.ipynb
│   ├── 11_Identity_Verification.ipynb
│   ├── 12_Synthetic_Diversity.ipynb
│   ├── 13_Final_Recognition_Model.ipynb
│   ├── 14_CrossDataset_Evaluation.ipynb
│   ├── 15_Explainability.ipynb
│   ├── 16_Ablation_Studies.ipynb
│   ├── 17_Performance_Comparison.ipynb
│   ├── 18_Statistical_Analysis.ipynb
│   ├── 19_Inference_Demo.ipynb
│   └── 20_Paper_Figures.ipynb
│
├── docs/
│   ├── Project_Report.pdf
│   └── Project_Presentation.pptx
│
├── requirements.txt
├── .gitignore
└── README.md
4. Research Workflow
The notebooks are designed to be executed in the following order:
Stage	Notebook(s)	Description
Dataset preparation	01–02	Dataset exploration and iris segmentation
Preprocessing	03–05	Normalization, enhancement and quality assessment
Few-shot learning	06–08	Dataset construction, baseline recognition and identity representation
Synthetic generation	09–10	Diffusion model training and synthetic image generation
Validation	11–12	Identity consistency and synthetic diversity analysis
Recognition	13–14	Final recognition and cross-dataset evaluation
Research analysis	15–18	Explainability, ablation, comparison and statistical analysis
Demonstration	19	End-to-end inference demonstration
Visualization	20	Generation of research paper figures
Important: The notebooks have dependencies on intermediate datasets, metadata, trained models and results produced by earlier stages. Execute them sequentially unless the required intermediate artifacts are already available.
5. Datasets
The project workflow currently references the following iris datasets:
CASIA-Iris-Thousand
IITD Iris Database
IITD dataset is not included in this because of liscence issue.
Users must obtain the datasets from their respective authorized sources and comply with their licensing, access and redistribution conditions.
Expected directory structure:
datasets/
└── raw/
    ├── CASIA-Iris-Thousand/
    └── IITD/
Place the authorized dataset files in their respective directories before executing the dataset exploration notebook.
Note: Dataset access may require registration or permission. Do not redistribute restricted biometric data through GitHub.
6. Software Requirements
The project uses Python and deep learning and image-processing libraries.
Recommended development environment:
Python 3.11
PyTorch
Torchvision
NumPy
Pandas
OpenCV
Pillow
Scikit-image
SciPy
Scikit-learn
Matplotlib
Jupyter Notebook
See requirements.txt for the project's Python dependencies.
GPU acceleration depends on the available hardware, operating system, NVIDIA driver and compatible PyTorch installation.
7. Installation and Environment Setup
Step 1: Clone the repository
git clone https://github.com/ashishya1206/Large-Scale-Aynthetic-Iris-Generation-For-Few-Shot-Generation
Step 2: Create a virtual environment
For Windows:
py -3.11 -m venv .venv
Activate:
.venv\Scripts\activate
For macOS/Linux:
python3.11 -m venv .venv
Activate:
source .venv/bin/activate
Step 3: Upgrade pip
python -m pip install --upgrade pip
Step 4: Install PyTorch
Install the appropriate PyTorch and Torchvision versions for your operating system and available hardware using the official installation selector:
https://pytorch.org/get-started/locally/
Step 5: Install project dependencies
pip install -r requirements.txt
Step 6: Register the Jupyter kernel
python -m ipykernel install --user --name iris-generation --display-name "Python (Iris Generation)"
Launch Jupyter:
jupyter notebook
Select the Python (Iris Generation) kernel.
8. Execution Instructions
1.Clone the repository.
2.Set up the Python environment and install the required dependencies.
3.Obtain the permitted datasets and place them in the expected directory structure.
4.Open the notebooks/ directory.
5.Execute the notebooks sequentially, beginning with 01_Dataset_Exploration.ipynb.
6.Verify the intermediate outputs before proceeding to subsequent stages.
7.Save experimental outputs, model checkpoints, generated images and evaluation metrics in their designated directories.
The notebooks contain configuration sections that allow parameters such as image limits, training settings, few-shot counts and evaluation options to be adjusted.
For initial testing, use the notebooks' quick-test settings where available before attempting full-scale experiments.
9. Reproducibility
To support reproducibility:
Maintain the same dependency versions across experiments.
Record dataset versions and preprocessing settings.
Preserve experiment configurations and random seeds.
Record training parameters and model checkpoint information.
Save evaluation metrics and generated figures.
Document any modifications to the experimental pipeline.
The final dependency versions and execution instructions will be updated after validation of the complete pipeline.


10. Project Documentation
The docs/ directory will contain:
Project report (PDF and editable document).
Project presentation slides.

The final project report and presentation will include a link to this GitHub repository.
11. Research Team
Role	Member
Student Researcher 1	Ashish Yadav
Student Researcher 2	Divyam Agrawal
Project Mentor	Dr. Meenakshi Choudhary
12. Repository Link
GitHub Repository:
https://github.com/YOUR_USERNAME/LargeScale_Synthetic_Iris_Generation
Replace the placeholder URL with the actual repository URL.
13. Acknowledgements and Dataset References
Dataset creators, research papers, pretrained models and other third-party resources will be acknowledged in the final project report and documented here as the implementation is finalized.
14. License and Data Usage
The repository's code and documentation are maintained for academic research and project evaluation.
Dataset redistribution and third-party model usage remain subject to their respective licenses and access conditions. No permission to redistribute third-party datasets is implied by this repository.
