# MD Simulation Free-State Analysis

This notebook provides an interactive workflow for the analysis of free-state molecular dynamics (MD) simulations, focusing on the calculation of Root Mean Square Deviation (RMSD) and sampling of glycosidic torsion angles.

## 📂 Repository Structure

- `MD_SIM_Analysis.ipynb`  
  Main notebook for data import, format conversion, RMSD analysis, and glycosidic angle sampling.
- `trajectory.xtc` (generated)  
  Trajectory file obtained from the conversion of a multimodel PDB file.
- `analysis_results/` (generated)  
  Folder containing the analysis results (plots, PDFs, raw data, etc.).

## 🛠️ Requirements

- Python 3.8 or higher
- [MDAnalysis](https://www.mdanalysis.org/)
- [mdtraj](https://mdtraj.org/)
- numpy
- matplotlib
- ipywidgets
- tqdm
- IPython

It is recommended to create a virtual environment (venv or conda) to isolate dependencies.

## ⚙️ Installation

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/MD-SIM-Analysis.git
cd MD-SIM-Analysis

# Create virtual environment with venv
env="mdsim-env"
python3 -m venv $env
source $env/bin/activate  # Linux/Mac
# .\$env\Scripts\activate  # Windows

# Install dependencies
pip install -r requirements.txt
