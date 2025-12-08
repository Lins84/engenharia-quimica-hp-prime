# HP Prime Thermodynamics Suite 🧪🔥

A comprehensive suite of high-precision Thermodynamic applications developed for the HP Prime Graphing Calculator using PPL (Prime Programming Language).

Designed for Chemical Engineers, Students, and Researchers, this suite runs natively on the calculator (no Python required) ensuring maximum speed and compatibility.

## 📦 Included Applications

The suite consists of 4 independent but complementary applications:

### 1. TERMO_TITANIUM (Pure Fluids EOS)
The core application for P-V-T calculations of pure substances.
* **Equations of State (EOS):** Ideal Gas, Van der Waals, Redlich-Kwong (RK), Soave-Redlich-Kwong (SRK), Peng-Robinson (PR), and Virial (Pitzer-Curl truncated).
* **Solver:** Includes a robust Newton-Raphson numerical solver to calculate **Temperature** (given P and V) or **Volume** (given P and T) for cubic equations, avoiding complex root ambiguity.
* **Advanced Properties:** Calculates Derivative Properties:
    * Compressibility Factor ($Z$)
    * Isobaric Thermal Expansivity ($\beta$)
    * Isothermal Compressibility ($\kappa$)

### 2. TERMO_MIX (Binary Mixtures)
Dedicated to Vapor-Liquid Equilibrium (VLE) parameters for binary mixtures.
* **Models:** SRK and Peng-Robinson.
* **Methodology:** Uses **van der Waals 1-fluid mixing rules**.
* **Features:**
    * Accepts Binary Interaction Parameter ($k_{ij}$).
    * Calculates Mixture parameters ($a_{mix}$, $b_{mix}$).
    * Outputs Mixture Volume ($V_{mix}$) and Compressibility ($Z_{mix}$).

### 3. TERMO_LIQ_PRO (Liquid Density)
 specialized tool for accurate liquid density/volume estimations.
* **Models:**
    * **Rackett (Estimated):** Uses Yamada-Gunn modification (requires only $T_c, P_c, \omega$).
    * **Rackett (Real $V_c$):** Uses experimental Critical Volume for higher precision.
    * **COSTALD:** (Hankinson-Thomson) The industry standard for compressed liquid density.
* **Reverse Solver:** Can calculate the Saturation Temperature given a specific Liquid Volume.

### 4. TERMO_GEN_PLUS (Generalized Charts)
A helper tool for using Lee-Kesler Generalized Compressibility Charts manually.
* **Pure Fluids:** Calculates Reduced Temperature ($Tr$) and Pressure ($Pr$).
* **Mixtures:** Implements **Kay's Rule** to calculate Pseudocritical Properties ($T_{pc}, P_{pc}$) and provides the correct coordinates for chart reading.

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

## ⚠️ Disclaimer

These programs are intended for educational and engineering reference purposes. While rigorous testing has been conducted against standard literature values (Perry's Handbook, NIST), the author assumes no responsibility for errors in critical professional applications. Always verify results.

---
*Developed by Leonardo Lins/Lins84/O cara da Prime*
