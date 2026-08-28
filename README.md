# IRCER-PDC-MLIP

This repository gathers reference databases, machine-learning interatomic potentials (MLIPs), and example input files developed for atomistic simulations of polymer-derived ceramics (PDCs) at IRCER.

The current release contains the Si-C-N-H database and MACE potential developed for the study of phase separation in polymer-derived silicon carbonitride ceramics.

## Repository contents

```text
IRCER-PDC-MLIP/
├── IRCER-PDC-DB/
│   └── IRCER-PDC-DB_v1.0.xyz
├── MLIPs/
│   ├── IRCER-SiCNH-MACE_v1.0.model
│   └── IRCER-SiCNH-MACE_v1.0.model-mliap_lammps.pt
├── Tools/
│   ├── cp2k_input.in
│   └── lammps_input.in
├── LICENSE
└── README.md
```

### Database

`IRCER-PDC-DB/IRCER-PDC-DB_v1.0.xyz`

Reference database used to train the Si-C-N-H MACE potential. The database contains atomic configurations with reference energies and forces obtained from first-principles calculations.

### Machine-learning interatomic potentials

`MLIPs/IRCER-SiCNH-MACE_v1.0.model`

Trained MACE model for Si-C-N-H systems.

`MLIPs/IRCER-SiCNH-MACE_v1.0.model-mliap_lammps.pt`

Model converted for use with LAMMPS through the MACE/ML-IAP interface.

### Example input files

`Tools/cp2k_input.in`

Example CP2K input file representative of the first-principles calculations used to generate reference data.

`Tools/lammps_input.in`

Example LAMMPS input file for molecular dynamics simulations using the released MACE potential.

## Citation

If you use this database, potential, or associated input files, please cite:

**Fabien Mortier, Sylvian Cadars, Olivier Masson, Mauro Boero, Guido Ori, Yun Wang, Samuel Bernard, and Assil Bouzid**,  
*Modeling phase separation in polymer-derived silicon carbonitride ceramics through extended machine learning molecular dynamics*,  
Journal:  
DOI:  

## Authors and affiliations

**Fabien Mortier, Sylvian Cadars, Olivier Masson, Samuel Bernard, Assil Bouzid**  
Institut de Recherche sur les Céramiques (IRCER), UMR 7315 CNRS-Université de Limoges, Centre Européen de la Céramique, 12 rue Atlantis, 87068 Limoges, France.

**Mauro Boero**  
University of Strasbourg, CNRS, ICube Laboratory UMR 7357, F-67412 Illkirch, France.  
ADYNMAT CNRS consortium, F-67034 Strasbourg, France.

**Guido Ori**  
ADYNMAT CNRS consortium, F-67034 Strasbourg, France.  
Université de Strasbourg, CNRS, Institut de Physique et Chimie des Matériaux de Strasbourg, UMR 7504, F-67034 Strasbourg, France.

**Yun Wang**  
Centre for Catalysis and Clean Energy, School of Environment and Science, Griffith University, Gold Coast, Australia.

Corresponding author: Assil Bouzid  
Email: assil.bouzid@cnrs.fr

## Version

Current release:

- `IRCER-PDC-DB v1.0`
- `IRCER-SiCNH-MACE v1.0`

Future PDC databases and MLIPs developed by the group may be added to this repository.

## License

This repository is distributed under the MIT License. See the [`LICENSE`](LICENSE) file for details.
