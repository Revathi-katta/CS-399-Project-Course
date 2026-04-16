# CS-399 Project Course  
## Spiking Neural Networks vs Artificial Neural Networks

This repository contains the implementation and analysis of **Spiking Neural Networks (SNNs)** and their comparison with **Artificial Neural Networks (ANNs)**. The project focuses on evaluating biologically inspired neuron models, such as **Leaky Integrate-and-Fire (LIF)** and **Multi-Synaptic Function (MSF)**, across various machine learning tasks.


##  Project Overview  

Spiking Neural Networks are considered a more biologically realistic alternative to traditional neural networks. In this project, we:

- Implemented **LIF (Leaky Integrate-and-Fire)** neuron models  
- Implemented **MSF (Multi-Synaptic Function)** neuron models  
- Applied these models to:
  - **Text Classification** (AG News dataset)  
  - **Image Classification** tasks  
- Compared their performance with standard **ANN models**  
- Analyzed differences in **accuracy, efficiency, and behavior**

---

## Key Concepts  

### 🔹 LIF Neuron
- Generates **one spike per timestep**
- Captures temporal behavior  
- Limited in representing input intensity  

### 🔹 MSF Neuron (Core Contribution)
- Allows **multiple spikes per timestep**
- Uses **multiple thresholds (Vth, 2Vth, …, D·Vth)**
- Captures:
  - Instantaneous intensity (rate coding)  
  - Temporal dynamics (spike timing)  

### 🔹 Surrogate Gradient Learning
- Enables training despite non-differentiable spike function  
- Ensures **stable gradient flow across layers**

---

## Results & Insights  

- MSF improves representation of **input intensity** over LIF  
- Stable training achieved using **surrogate gradients**  
- SNNs demonstrate potential for **NLP tasks with temporal encoding**  
- Energy estimation (45nm CMOS model):
  - ANN: **4.6 pJ (MAC)**  
  - SNN: **0.9 pJ (AC)** scaled by firing rate  

---

##  Technologies Used  

- Python  
- PyTorch  
- Jupyter Notebook  
- NumPy  
- Matplotlib  

---

##  Instructor  
**Prof. Manisha Padala**

---

##  Contributors  
**Chepuri Venkata Naga Thrisha (23110079)**  
**Katta Revathi (23110159)**   
B.Tech @ IIT Gandhinagar

---
