# FeNNol Pre-trained Models Collection
This repository contains a collection of pre-trained models compatible with the [FeNNol library](https://github.com/thomasple/FeNNol).

## Available models
- ANI1x, ANI1ccx, ANI2x 
- MACE-OFF23 (small, medium, large)
- MACE-MP (small, medium, large)

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