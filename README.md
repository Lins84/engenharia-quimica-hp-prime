# HP Prime Thermodynamics Suite 🧪🔥 

A comprehensive suite of high-precision Thermodynamic applications developed for the HP Prime Graphing Calculator using PPL (Prime Programming Language).

Designed for Chemical Engineers, Students, and Researchers, this suite runs natively on the calculator (no Python required) ensuring maximum speed and compatibility.

## 📦 Included Applications

The suite consists of 4 independent but complementary applications:


<img width="320" height="240" alt="Menu TERMOTITANIUM" src="https://github.com/user-attachments/assets/049747ad-def5-4660-a04a-98c16af968f5" />


### 1. TERMO_TITANIUM (Pure Fluids EOS)
The core application for P-V-T calculations of pure substances.
* **Equations of State (EOS):** Ideal Gas, Van der Waals, Redlich-Kwong (RK), Soave-Redlich-Kwong (SRK), Peng-Robinson (PR), and Virial (Pitzer-Curl truncated).
* **Solver:** Includes a robust Newton-Raphson numerical solver to calculate **Temperature** (given P and V) or **Volume** (given P and T) for cubic equations, avoiding complex root ambiguity.
* **Advanced Properties:** Calculates Derivative Properties:
    * Compressibility Factor ($Z$)
    * Isobaric Thermal Expansivity ($\beta$)
    * Isothermal Compressibility ($\kappa$)

<img width="320" height="240" alt="BETA KAPPA" src="https://github.com/user-attachments/assets/3da270b5-b604-42d3-8a0c-63c2adaf6482" />      <img width="320" height="240" alt="KAPPA3" src="https://github.com/user-attachments/assets/c7bf8d8e-c17a-4b79-bdca-dbae613020f1" />




### 2. TERMO_MIX (Binary Mixtures)
Dedicated to Vapor-Liquid Equilibrium (VLE) parameters for binary mixtures.
* **Models:** SRK and Peng-Robinson.
* **Methodology:** Uses **van der Waals 1-fluid mixing rules**.
* **Features:**
    * Accepts Binary Interaction Parameter ($k_{ij}$).
    * Calculates Mixture parameters ($a_{mix}$, $b_{mix}$).
    * Outputs Mixture Volume ($V_{mix}$) and Compressibility ($Z_{mix}$).
 

<img width="320" height="240" alt="MIX3" src="https://github.com/user-attachments/assets/b29ce1f1-ef91-4dcc-a493-77f6d7d2eb29" /> <img width="320" height="240" alt="MIX2" src="https://github.com/user-attachments/assets/c7b5887b-44a5-424f-8377-6d6b036ad162" />



### 3. TERMO_LIQ_PRO (Liquid Density)
 specialized tool for accurate liquid density/volume estimations.
* **Models:**
    * **Rackett (Estimated):** Uses Yamada-Gunn modification (requires only $T_c, P_c, \omega$).
    * **Rackett (Real $V_c$):** Uses experimental Critical Volume for higher precision.
    * **COSTALD:** (Hankinson-Thomson) The industry standard for compressed liquid density.
* **Reverse Solver:** Can calculate the Saturation Temperature given a specific Liquid Volume.


<img width="320" height="240" alt="LIQUID" src="https://github.com/user-attachments/assets/6e372fc6-b82b-4748-90eb-56ee3efe3179" /> <img width="320" height="240" alt="image" src="https://github.com/user-attachments/assets/dbecab08-72d8-4b88-9ff3-23a41a713051" />




### 4. TERMO_GEN_PLUS (Generalized Charts)
A helper tool for using Lee-Kesler Generalized Compressibility Charts manually.
* **Pure Fluids:** Calculates Reduced Temperature ($Tr$) and Pressure ($Pr$).
* **Mixtures:** Implements **Kay's Rule** to calculate Pseudocritical Properties ($T_{pc}, P_{pc}$) and provides the correct coordinates for chart reading.



<img width="320" height="240" alt="image" src="https://github.com/user-attachments/assets/414b5c7a-dabc-40e1-96a5-566d8593201a" /><img width="320" height="240" alt="image" src="https://github.com/user-attachments/assets/dcce9c64-59dc-4dca-9ce1-fcb250c3f2a7" /><img width="320" height="240" alt="image" src="https://github.com/user-attachments/assets/ebdc1b89-45cb-4e9a-aa14-40ea3790dde5" />





---

## 🚀 Installation

1.  Download the **HP Connectivity Kit** from the official HP website.
2.  Connect your HP Prime calculator to your PC via USB.
3.  Download the `.ppl` files from this repository.
4.  Open the `.ppl` files (as text) and copy the code.
5.  In the Connectivity Kit:
    * Right-click on **"Programs"** (or "Program Library").
    * Select **"New Program"**.
    * Name it exactly as the file (e.g., `TERMO_TITANIUM`).
    * Paste the code and save.
6.  The App will appear in your calculator's **Program Catalog** (`Shift` + `1`).

## 📖 How to Use

1.  Press `Shift` + `1` (Program) on your calculator.
2.  Select the desired App (e.g., `TERMO_TITANIUM`) and press **Run**.
3.  **Menu Navigation:** Use the touchscreen or numbers to select Models and Calculation Objectives.
4.  **Inputs:** The apps use Global Variables (`EXPORT`). Once you enter data for a substance (e.g., Water: $Tc=647.1, Pc=220.6$), it stays saved in memory for subsequent calculations, saving you typing time.
5.  **Escape:** Press `Esc` in menus to go back or exit.

## 📺 YouTube Channel (Coming Soon)
I recently started a channel dedicated to HP Prime engineering tutorials.
**Subscribe now to be the first to know when the full video manual for this suite is released!**

[**🔗 Click here to Subscribe**](https://www.youtube.com/@ocaradaprime)


## ⚠️ Disclaimer

These programs are intended for educational and engineering reference purposes. While rigorous testing has been conducted against standard literature values (Perry's Handbook, NIST), the author assumes no responsibility for errors in critical professional applications. Always verify results.

---
*Developed by Leonardo Lins*
