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

# Create virtual environment with venv
env="mdsim-env"
python3 -m venv $env
source $env/bin/activate  # Linux/Mac
# .\$env\Scripts\activate  # Windows

# Install dependencies
pip install -r requirements.txt
```
##  🚀 Usage

-  Start Jupyter Notebook:

    ```jupyter notebook```

-  Open `MD_SIM_Analysis.ipynb` in your browser.

-  Execute the cells in order:

  1. Load dependencies

  2.  Convert multimodel PDB file to trajectory.xtc

  3.  RMSD analysis with widget interface

  4. Glycosidic torsion angle sampling

-  All plots and results will be saved in the analysis_results/ folder.

##  📝 Section Description

-  Load necessary dependencies: imports libraries and modules.

-  Multimodel.pdb → trajectory.xtc Converter: converts a multimodel PDB file into a usable XTC trajectory file.

-  Root Mean Square Deviation (RMSD) Analysis: calculates and visualizes RMSD relative to a reference structure.

-  Glycosidic Torsion Angle Sampling: performs distributional sampling of glycosidic angles (phi/psi) throughout the simulation.

##  📈 Results

Interactive plots within the notebook

Automatic export to PNG, SVG, PDF via matplotlib

##  🤝 Contributing

Pull requests and issues are welcome! To contribute:

-  Fork the repository

-  Create a branch (git checkout -b feature/my-feature)

-  Commit your changes (git commit -m "Add...")

-  Push to the branch (git push origin feature/my-feature)

-  Open a Pull Request

🙏 Acknowledgments

This workflow draws inspiration from similar MD analysis pipelines. If you find this workflow useful, please consider sharing it with your colleagues, research network, or anyone interested in glycochemistry MD analysis. Your support helps the community grow!

📜 License

This project is licensed under the MIT License. See LICENSE for more information.
