# FeNNol Pre-trained Models Collection
This repository contains a collection of pre-trained models compatible with the [FeNNol library](https://github.com/thomasple/FeNNol).

## Available models
- FeNNix-Bio1 (**AVAILABLE SOON !**)
- ANI1x, ANI1ccx, ANI2x 
- MACE-OFF23 (small, medium, large)
- MACE-MP (small, medium, large)

## Installation
In order to get the model files (files with `.fnx` extensions), you can either clone this repository or download the desired model directly from the github interface.

*Warning:* Models larger than 100MB are stored using Git LFS. If you clone the repository and want to use these models, make sure to have Git LFS installed on your system.

## Usage
To use the models, simply download the desired model and load it using the FeNNol library. For example, to load the MACE-OFF23 small model in an ASE calculator, use the following code:
```python
from fennol.ase import FENNIXCalculator
from ase import build

atoms = build.molecule('H2O')
calc = FENNIXCalculator(model='MACE-OFF23/mace_off_small.fnx')
atoms.calc = calc
print("energy =",atoms.get_potential_energy())
```

## Citation

If you use any of the models provided in this repository, please cite the corresponding papers. Please also cite this paper if you use the FeNNol library.
```
T. Plé, O. Adjoua, L. Lagardère and J-P. Piquemal. FeNNol: an Efficient and Flexible Library for Building Force-field-enhanced Neural Network Potentials. arXiv preprint arXiv:2405.01491 (2024)
```

```bib
@article{ple2024fennol,
  title={FeNNol: an Efficient and Flexible Library for Building Force-field-enhanced Neural Network Potentials},
  author={Pl{\'e}, Thomas and Adjoua, Olivier and Lagard{\`e}re, Louis and Piquemal, Jean-Philip},
  journal={arXiv preprint arXiv:2405.01491},
  year={2024}
}
```

## Licence
Each model family is distributed under its own licence. Please refer to the corresponding model folder for more information.