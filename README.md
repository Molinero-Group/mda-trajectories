# MDA: Compression, Decompression, and Shear Deformation of Amorphous Ice

This repository contains molecular dynamics trajectories used to study the response of amorphous ice to **compression, decompression, and shear deformation** using the **ML-BOP water potential**.

The simulations contain **8,000 water particles** and are associated with the analysis presented in:

**I. de Almeida Ribeiro, D. Dhabal, R. Kumar, S. Banik, S. K. R. S. Sankaranarayanan, and V. Molinero**,
*Medium-density amorphous ice unveils shear rate as a new dimension in water's phase diagram*,
**Proceedings of the National Academy of Sciences 121, e2414444121 (2024).**
DOI: **10.1073/pnas.2414444121**

Paper: https://www.pnas.org/doi/abs/10.1073/pnas.2414444121

## Repository contents

The repository is organized according to the deformation protocol:

```text
mda/
├── compress/
├── decompress/
└── under-shear/
```

## Simulation details

* **System:** Water
* **Number of particles:** 8,000
* **Interaction model:** ML-BOP water potential
* **Simulation method:** Molecular dynamics
* **Trajectory format:** LAMMPS dump files
* **Trajectory file:** `dump.atom`
* **Thermodynamic data:** `ave.log`
* **LAMMPS input:** The corresponding LAMMPS input file is included in each simulation directory.

For the **shear simulations**, the top-level directory names indicate the applied **shear rate**. Within each shear-rate directory, the simulations are further organized according to the **initial structure** and the **pressure imposed during the NPT simulation under shear**.

Thus, each simulation directory contains the files needed to reproduce or analyze the corresponding trajectory, including the atomic trajectory (`dump.atom`), thermodynamic data (`ave.log`), and LAMMPS input.

The trajectories can be visualized and analyzed using software such as **OVITO**, or processed directly using Python or other molecular simulation analysis tools.

For the detailed simulation protocols, thermodynamic conditions, deformation rates, structural analysis, and interpretation of the results, please refer to the paper and its Supporting Information.

## Citation

If you use these trajectories or data in your work, please cite:

> de Almeida Ribeiro, I.; Dhabal, D.; Kumar, R.; Banik, S.; Sankaranarayanan, S. K. R. S.; Molinero, V.
> **Medium-density amorphous ice unveils shear rate as a new dimension in water's phase diagram.**
> *Proceedings of the National Academy of Sciences* **121**, e2414444121 (2024).
> DOI: 10.1073/pnas.2414444121
