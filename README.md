# Integrating Graph Neural Networks and Molecular Docking to Predict Xylopia aethiopica Compounds’ Anti-Breast Cancer Activity 

---

## Overview
This repository presents a **computational-driven framework** that integrates **Graph Neural Networks (GNNs)** and **molecular docking** to predict the **inhibitory activity of phytocompounds derived from *Xylopia aethiopica*** against the **Human Estrogen Receptor Alpha (ERα)**—a major therapeutic target in **estrogen receptor–positive (ER⁺) breast cancer**.

The project bridges **cheminformatics**, **machine learning**, and **structural biology**, demonstrating how **graph-based molecular representations** can be utilized to discover natural compounds with potential **anti-breast cancer properties**.

---

## 🧠 Biological Relevance
Breast cancer remains one of the most prevalent cancers in women, with over 70% of cases classified as **estrogen receptor–positive (ER⁺)**. In these tumors, the **Human Estrogen Receptor Alpha (ERα)** acts as a transcription factor that, when activated by **estrogen**, drives abnormal cell growth and tumor progression.

Therapies that inhibit ERα—such as **Tamoxifen** and **Fulvestrant**—are effective but often limited by **side effects** and **resistance**. To address these limitations, this study investigates ***Xylopia aethiopica*** phytochemicals as **natural inhibitors** of ERα. By combining **Graph Neural Networks** for predictive modeling with **molecular docking** for validation (using **PDB ID: 2IOK**), this research aims to identify new plant-derived compounds capable of binding and suppressing ERα activity, offering a promising pathway for **natural, low-toxicity breast-cancer therapeutics**.

---

## ⚗️ Research Highlights
- 🧩 **Graph Neural Network (GNN)** modeling for predicting inhibitory activity  
- ⚛️ **Molecular docking** validation of *Xylopia aethiopica* phytocompounds against ERα (PDB ID: 2IOK)  
- 🌿 **Natural product-based inhibitor discovery** targeting breast-cancer pathways  
- 📊 Visualization of docking poses, interaction maps, and performance metrics  

---

## ⚙️ Workflow

1. **Data Preparation:** Collection and curation of *Xylopia aethiopica* phytochemical data  
2. **Feature Engineering:** Generation of molecular graphs and fingerprints  
3. **Model Training:** GNN architecture for regression/classification of inhibitory potency  
4. **Virtual Screening:** Prediction of high-affinity ERα inhibitors  
5. **Docking Validation:** Docking of top-ranked compounds with receptor structure (2IOK)  
6. **Analysis & Visualization:** Binding affinity analysis, hydrogen-bond mapping, and result interpretation  

---

## 📁 Repository Structure
| Folder | Description |
|:--|:--|
| `data/` | Raw and processed datasets of phytochemicals |
| `notebooks/` | Jupyter notebooks for preprocessing, model training, and analysis |
| `test_checkpoints_reg/` | Trained GNN models and configuration files |
| `images/` | Figures, molecular interaction plots, and workflow diagrams |

---

## 📊 Model Performance

<p align="center">
  <img src="https://github.com/Izuagba/GNN-Xylopia-aethiopica-BreastCancer/blob/main/images/Train_GNN_Rmse.png" width="30%"/>
  <img src="https://github.com/Izuagba/GNN-Xylopia-aethiopica-BreastCancer/blob/main/images/Val_GNN_Rmse.png" width="30%"/>
  <img src="https://github.com/Izuagba/GNN-Xylopia-aethiopica-BreastCancer/blob/main/images/Test_GNN_Rmse.png" width="30%"/>
</p>

<p align="center"><em>Training, validation, and testing RMSE performance of the GNN model.</em></p>

---

## 🧪 Docking & Interaction Visualizations

<p align="center">
  <img src="https://github.com/Izuagba/GNN-Xylopia-aethiopica-BreastCancer/blob/main/images/Cocrystallised_protein_interaction.png" width="45%"/>
  <img src="https://github.com/Izuagba/GNN-Xylopia-aethiopica-BreastCancer/blob/main/images/tamoxifen_protein_interaction.png" width="45%"/>
</p>

<p align="center"><em>(Left) Cocrystallized ERα interaction. (Right) Standard drug Tamoxifen–ERα interaction.</em></p>

<p align="center">
  <img src="https://github.com/Izuagba/GNN-Xylopia-aethiopica-BreastCancer/blob/main/images/Human%20estrogen%20receptor%20alpha%20ligand-binding%20domain%20in%20complex%20with%20compound%201D%20.png" width="45%"/>
  <img src="https://github.com/Izuagba/GNN-Xylopia-aethiopica-BreastCancer/blob/main/images/REDOCK-SUPERPOSITION.png" width="45%"/>
</p>

<p align="center"><em>(Left) Xylopia aethiopica compound (1D) bound to ERα. (Right) Superposition of docked and redocked structures.</em></p>

---

## 🧬 Structural Validation

<p align="center">
  <img src="https://github.com/Izuagba/GNN-Xylopia-aethiopica-BreastCancer/blob/main/images/Ramanchadan.png" width="50%"/>
</p>

<p align="center"><em>Ramachandran plot confirming stereochemical stability of the ERα model.</em></p>

---

## ⚙️ Tools & Frameworks

| Category | Tools |
|-----------|-------|
| **Programming & Modeling** | Python 3, PyTorch Geometric, Chemprop, Scikit-learn |
| **Cheminformatics** | RDKit, PaDEL-Descriptor |
| **Docking & Visualization** | Maestro Schrodinger Software |
| **Data Processing** | NumPy, Pandas, Matplotlib, Seaborn |

## ✍️ Author

**Izuagba Favour Ogadinma**  
Research Assistant | Chemsolvers and Computational Research Laboratories
[LinkedIn](https://www.linkedin.com/in/izuagba-favour-ogadinma) • [GitHub](https://github.com/Izuagba)

---

🧾 Citation

If you use this repository, please cite:

Izuagba Favour Ogadinma (2025). Integrating Graph Neural Networks and Molecular Docking to Predict the Inhibitory Activity of Xylopia aethiopica Phytocompounds against Human Estrogen Receptor Alpha in Breast Cancer.

## 📜 License
This project is licensed under the [MIT License](LICENSE).

---

## 🧩 Installation

```bash
# Clone this repository
git clone https://github.com/<your-username>/XylopiaGNN-ERalpha.git
cd XylopiaGNN-ERalpha

# Create environment
conda create -n xylopia_gnn python=3.10
conda activate xylopia_gnn

