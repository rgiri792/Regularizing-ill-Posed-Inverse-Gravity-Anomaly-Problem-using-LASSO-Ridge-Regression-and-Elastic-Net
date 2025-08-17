# 🌍 Gravity Inverse Problem  

This repository contains a **Jupyter Notebook** that demonstrates the solution of the **Gravity Inverse Problem**. The gravity inverse problem is a fundamental geophysical challenge: given gravitational anomaly measurements at the surface, estimate the underlying subsurface density distribution.  

---

## 📌 Project Description  

The **gravity inverse problem** is central to geophysical exploration and Earth sciences. Unlike the forward problem (where the gravitational field is calculated from a known mass distribution), the inverse problem seeks to determine **unknown density distributions** from observed gravity anomalies. This is inherently **ill-posed**, meaning multiple subsurface models can explain the same surface measurements.  

This project illustrates techniques to approach the inverse problem by formulating it as a **matrix inversion problem**. The methodology involves:  

1. **Forward Gravity Model**  
   - Computes gravitational anomalies at the surface from subsurface density distributions.  

2. **System Representation**  
   - Pressure/gravity data is expressed in linear algebraic form:  
     \[
     \mathbf{d} = \mathbf{Gm}
     \]  
     where **d** is observed data, **G** is the forward operator (sensitivity matrix), and **m** is the model vector (density distribution).  

3. **Inverse Solution**  
   - Estimates the model vector **m** using inversion techniques.  
   - Handles non-uniqueness via **regularization** and **stabilization strategies**.  

4. **Error Analysis**  
   - Compares reconstructed gravity data with observed anomalies.  

5. **Visualization**  
   - Provides intuitive plots of input data, predicted anomalies, and recovered density distributions.  

This notebook is designed as a **teaching and exploration tool**, helping to understand the ill-posed nature of geophysical inverse problems while experimenting with mathematical inversion methods.  

---

## ⚙️ Features  
- Implementation of forward gravity model  
- Linear algebraic formulation of the inverse problem  
- Regularization techniques for stabilizing solutions  
- Visualization of anomalies and reconstructed density fields  
- Clear workflow for educational and research purposes  

---

## 🔧 Requirements  
Make sure you have the following Python packages installed:  
```txt
numpy  
matplotlib  
scipy  
jupyter  
git clone https://github.com/<your-username>/Gravity-Inverse-Problem.git
cd Gravity-Inverse-Problem
jupyter notebook Gravity_Inverse_Problem_v2.ipynb
