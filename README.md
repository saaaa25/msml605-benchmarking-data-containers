# 🚀 **Benchmarking Data Containers: NumPy vs. PyTorch vs. C++**  
*Explore performance of NumPy, PyTorch, and C++ data containers. Analyze CPU and GPU efficiency across key algorithms and tasks.*  

---

## 📋 **Table of Contents**  
- [Prerequisites](#-prerequisites)  
- [Setup](#-setup-in-google-colab)  
- [Usage](#-usage)  
- [Troubleshooting](#-troubleshooting)  
- [License](#-license)  

---

## 🔧 **Prerequisites**  
Before running this notebook, ensure you have:  
- A **Google account** (to access [Google Colab](https://colab.research.google.com/)).  
- The **`.ipynb` file** (uploaded to Google Drive/GitHub or locally stored).  

---

## ⚙️ **Setup in Google Colab**  

### **Option 1: Open from GitHub**  
1. Go to [Google Colab](https://colab.research.google.com/).  
2. Click the **GitHub** tab.  
3. Paste this repository URL or `.ipynb` file link → Press **Enter**.  

### **Option 2: Upload Manually**  
1. Open [Google Colab](https://colab.research.google.com/).  
2. Click **File** → **Upload notebook** → Select your `.ipynb` file.  

---

## 🎯 **Usage**  
1. **Set Runtime**:  
   - Click **Runtime** → **Change runtime type** → Select **Python 3** + **GPU/TPU** (if needed).  

2. **Install Dependencies**:  
   ```python
   !pip install numpy pandas tensorflow
   import cupy as cp
   import torch  # Main PyTorch library (includes CUDA support)
   import time trace_malloc #for performance metrics
   
3. **Download Images**:  
   - for image preprocessing performance metrics
   - upload these images in Sample data folder before running the code.
  
4. **Required Headers (C++/CUDA Files)**:

   - For any custom CUDA kernels or low-level operations, your C++/CUDA files must include these headers:
   ```cpp
   // Core CUDA runtime functionality (memory management, device functions)
   #include <cuda_runtime.h>

   // PyTorch C++/CUDA extension support (if integrating with PyTorch)
   #include <torch/extension.h>


