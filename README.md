# CRAFT Model – README

## 1. Model Overview

We develop **CRAFT** (*Chemical Regional Analysis Framework for low-carbon Transition*), a spatially explicit and integrated modelling framework that links **resources, technologies, costs, and transition risks** in China’s chemical sector.

CRAFT covers major primary chemicals and optimizes **provincial decarbonization pathways from 2020 to 2060**. It follows a **capacity-expansion modelling structure**, minimizing total system cost by jointly optimizing technology deployment and operation under provincial resource potentials, carbon emission constraints and product demand requirements.

The model explicitly represents the production of **ammonia, methanol, high-value chemicals (HVCs: ethylene, propylene, and aromatics)**, as well as **hydrogen for refining**. It includes both:

- **Conventional routes** based on coal, natural gas, and oil  
- **Low-carbon routes** relying on green hydrogen, biomass, and carbon capture and storage (CCS)

Through this integrated structure, CRAFT enables a consistent assessment of cost-effective and regionally differentiated low-carbon transition pathways for the chemical industry.

---

## 2. Directory Structure

To run the model properly, the root directory must contain the following folders and files:

root/

│

├─ venv/ # Python virtual environment

├─ model_code/ # Model code written in Python (Jupyter Notebook format)

│

├─ indices.xlsx # Index file defining model dimensions and mappings

├─ data.xlsx # Core dataset required by the model

├─ 00_readme.xlsx # Detailed documentation of each sheet in data.xlsx

│

├─ S.../ # Result storage folder (scenario S...)




- **`venv/`** contains the required Python virtual environment.  
- **`model_code/`** stores the Jupyter Notebook implementing the CRAFT model logic.  
- **`indices.xlsx`** defines model indices and structural mappings.  
- **`data.xlsx`** provides all numerical inputs required for model execution.  
- **`00_readme.xlsx`** documents the content, units, and meaning of each sheet in `data.xlsx`.  
- **`S.../`** are used to store outputs for different scenarios. You need to create the folder yourself, for example: S0. 

---

## 3. Execution Requirements (Important)

Please carefully check the following requirements before running the model:

**a. Python version**  
- Executing the model requires **Python 3.8.5**.

**b. Virtual environment**  
- The **virtual environment must be activated** before running the code.

**c. Output folders**  
- Result storage folders such as **S0, S1, S2, S3** must be created in the root directory in advance.  
- If these folders do not exist, **model results cannot be saved**.

**d. Solver license**  
- Running the model requires a **Gurobi commercial (professional) license**.  
- The **free Gurobi license is insufficient** to support the large-scale optimization problems solved in CRAFT.
