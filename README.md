# GLYtool (beta version)
Project created to provide valuable rapid analysis tools in the field of glycoscience. The project consists of several Jupiter Notebook. This allows the analyses to be reproduced, executed on any operating system and made simple for all users, even those with less experience. The project is currently under development, so please be kind and notify me of any errors :)
This notebook provides an interactive workflow for the analysis of free-state molecular dynamics (MD) simulations, focusing on the calculation of Root Mean Square Deviation (RMSD) and sampling of glycosidic torsion angles.

## 📂 Repository Structure

- `FreeSimGLY.ipynb`  
  Main notebook for free-state molecular dynamic simulations, composed by format conversion, RMSD and RMSF analysis, glycosidic angle sampling and clusterization of poses obtained.
- `BoundSimGLY.ipynb`
  Coming soon
- `Requirements.txt`
  File to easy-to-install requirement dependencies.

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
git clone https://github.com/YOUR_USERNAME/GLYtool-Beta.git
cd GLYtool-Beta

# Create virtual environment with venv
env="GLYtool-env"
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

-  Open `FreeSimGLY.ipynb` in your browser.

-  Execute the cells in order:

  1. Load dependencies

  2.  Convert multimodel PDB file to trajectory.xtc

  3.  RMSD analysis with widget interface

  4. Glycosidic torsion angle sampling
     
  5. Pose Clusterization 


##  📝 Section Description

-  Multimodel.pdb → trajectory.xtc Converter: converts a multimodel PDB file into a usable XTC trajectory file.

-  Root Mean Square Deviation (RMSD) and Root Mean Square Fluctuation (RMSF) Analysis: calculates and visualizes RMSD and RMSF relative to a reference structure.

-  Glycosidic Torsion Angle Sampling: performs distributional sampling of glycosidic angles (phi/psi) throughout the simulation.

-  Clustering of dynamics: This allows you to select the number of representative poses to be extrapolated, after which a clustering report is returned, representing each pose    and sampled frame.

##  📈 Results

Interactive plots within the notebook

Automatic export to PNG, SVG, PDF via matplotlib

You can then download the generated clustering PDB files to a dedicated folder

##  🤝 Contributing

Pull requests and issues are welcome! To contribute:

-  Fork the repository

-  Create a branch (git checkout -b feature/my-feature)

-  Commit your changes (git commit -m "Add...")

-  Push to the branch (git push origin feature/my-feature)

-  Open a Pull Request

🙏 Acknowledgments

This workflow draws inspiration from similar MD analysis pipelines. If you find this workflow useful, please consider sharing it with your colleagues, research network, or anyone interested in glycochemistry MD analysis. Your support helps the community grow!
