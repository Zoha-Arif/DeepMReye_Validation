# DeepMReye Validation

A validation project for **[DeepMReye](https://github.com/DeepMReye/DeepMReye)**, a neuroimaging tool that uses deep learning to estimate gaze positions directly from functional MRI (fMRI) data. Our primary aim is to compare DeepMReye’s gaze predictions with traditional eye-tracking measurements to assess accuracy and reliability.

---

## Table of Contents
1. [Onboarding Documentation](#onboarding-documentation)  
2. [Prerequisites](#prerequisites)  
3. [Installation](#installation)  
4. [Data Access](#data-access)  
5. [Project Structure](#project-structure)  
6. [Contributing](#contributing)  
7. [License](#license)  

---

## Onboarding Documentation

Below are some essential resources and references to help you get started:

- **fMRI Basics**: [Andy's Brain Book: Introduction to fMRI](https://andysbrainbook.readthedocs.io/en/latest/fMRI_Short_Course/fMRI_Intro.html)  
- **Introduction to Neural Networks and Deep Learning**: [3Blue1Brown Youtube Series](https://www.youtube.com/watch?v=aircAruvnKk&list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi) 

**Additional Documentation and Links:**
- [DeepMReye Repository](https://github.com/DeepMReye/DeepMReye)  
- [DeepMReye Example Usage Notebook](https://github.com/DeepMReye/DeepMReye/blob/main/notebooks/deepmreye_example_usage.ipynb)  
- [BIDS-MReye (Alternative Repo)](https://github.com/cpp-lln-lab/bidsMReye)  
- [DeepMReye Nature Neuroscience Paper](https://www.nature.com/articles/s41593-021-00947-w)  

---

## Prerequisites

Ensure you have the following installed or available:

- **Python 3.8+**  
- **Jupyter Notebooks**: [Download & Registration](https://jupyter.org/install)  
- **Git** (for version control)  
- (Optional) **Anaconda/Miniconda** (recommended for managing Python environments)

---

## Installation

Follow these steps to set up the project environment:

```bash
# 1. Clone the DeepMReye Validation repository
git clone https://github.com/Zoha-Arif/DeepMReye_Validation.git
cd DeepMReye_Validation

# 2. Clone the main DeepMReye repository (if needed)
git clone https://github.com/DeepMReye/DeepMReye.git

# 3. Create and activate a Python virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# 4. Install dependencies
pip install -r requirements.txt  # Adjust path if your requirements.txt is located elsewhere
```
## Data Access

This project uses both **example data from DeepMReye** and **project-specific datasets** to compare fMRI-derived gaze with traditional eye-tracking.

### Data Sources

1. **DeepMReye Sample Data**  
   - [OSF Link](https://osf.io/mrhk9/)  
   - Example dataset you can use to test if DeepMReye is set up correctly.

2. **LAND Lab Data (Vanderbilt University)**  
   - [OSF Link](https://osf.io/suak8/)  
   - Contains both fMRI and corresponding in-bore eye-tracking data for direct comparison.

### Example 1: Using `dipy` to Download a Public Dataset
```python
from dipy.data import fetch_stanford_t1
t1_fname = fetch_stanford_t1()
print(t1_fname)  # Location of downloaded data
