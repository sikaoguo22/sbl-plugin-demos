# sbl-plugin-demos
This repository contains a Pixi-based project that sets up all dependencies needed to experiment with the Structural Bioinformatics Library (SBL) and its plugins in a fully reproducible way. It provides:
- A Pixi manifest (pixi.toml) describing the environment, including JupyterLab, pixi-kernel, SBL runtime dependencies.
- Simple installation instructions to install SBL following the official installation guide.
- A set of Jupyter notebooks demonstrating how to run SBL plugins on different molecular viewer (VMD, PyMOL, NGL viewer in Web).
- The goal is to serve as an shareable demo for new users, collaborators, and reviewers to quickly test SBL plugins without manual environment debugging.

## Resources
- [SBL Home Page](https://sbl.inria.fr/) – Official website
- [SBL Documentation](https://sbl.inria.fr/doc/) – Online documentation
- [SBL YouTube Channel](https://www.youtube.com/channel/UClOhr0YMDkglcMKN5ZkMPnQ) – Video tutorials and demos

## Per-platform setup
1. Pick the `envs/<platform>/pixi.toml` matching your machine (`linux-64`, `osx-64`, `osx-arm64`). For Windows users, use the `linux-64` version within WSL. 
2. Create a new Pixi workspace (for example at `~/envs/sbl-pixi`) and place the chosen `pixi.toml` in that directory.  
3. Use Pixi to install the environment and then follow the steps in `notebooks/01_install_sbl_with_pixi.ipynb` to install and configure SBL plugins.

## SBL plugins
**Key features**

- Seamless integration with different molecular viewers
- Consistent usage across platforms
- Interactive analysis and visualization
- All plugins are automatically generated

### sbl-vorlume-pdb
**[Computing surface area and volume of a molecule](https://sbl.inria.fr/doc/Space_filling_model_surface_volume-user-manual.html)**

[Usage instructions](notebooks/02_sbl_vorlume_pdb.ipynb)

### sbl-bif-chainW-atomic
**[Interfaces and interactions within macro-molecular complexes](https://sbl.inria.fr/doc/Space_filling_model_interface_finder-user-manual.html)**

[Usage instructions](notebooks/03_sbl_bif_chainw_atomic.ipynb)

### sbl-intervor-ABW-atomic
**[Dissecting macro-molecular interfaces](https://sbl.inria.fr/doc/Space_filling_model_interface-user-manual.html)**

[Usage instructions](notebooks/04_sbl_intervor_abw_atomic.ipynb)

### sbl-kpax-iterative-alignment
**[Reference structural aligner](https://sbl.inria.fr/doc/Kpax-user-manual.html)**

[Usage instructions](notebooks/05_sbl_kpax.ipynb)

### sbl-misa
**[Combining MSA and interface models](https://sbl.inria.fr/doc/Multiple_interface_string_alignment-user-manual.html)**

[Usage instructions](notebooks/06_sbl_misa.ipynb)

### sbl-spectraldom
**[Defining domains within a polypeptide chain or protein](https://sbl.inria.fr/doc/Spectral_domain_explorer-user-manual.html)**

[Usage instructions](notebooks/07_sbl_spectraldom.ipynb)

### sbl-tripeptide-loop-closure
**[Generate or modify tripeptide segments in protein structure](https://sbl.inria.fr/doc/Tripeptide_loop_closure-user-manual.html)**

[Usage instructions](notebooks/08_sbl_tlc.ipynb)

### sbl-alphafold-dbrun
**[Characterizing the fragmentation of alphafold predictions](https://sbl.inria.fr/doc/Alphafold_analysis-user-manual.html)**

[Usage instructions](notebooks/09_sbl_afdb.ipynb)