# MACE-OFF23 models

This folder contains the MACE-OFF23 pre-trained transferable organic force fields from 

    Dávid Péter Kovács et al., MACE-OFF23: Transferable Machine Learning Force Fields for Organic Molecules, arXiv:2312.15211 (2023)

https://doi.org/10.48550/arXiv.2312.15211

These models come in three sizes:
 - small --> `mace_off_small.fnx`
 - medium --> `mace_off_medium.fnx`
 - large --> `mace_off_large.fnx`

All the models have been converted to `.fnx` format from the corresponding pytorch models provided in the [MACE repository](https://github.com/ACEsuit/mace) and the [MACE-OFF repository](https://github.com/ACEsuit/mace-off).

*Warning*: the file `mace_off_large.fnx` is stored using Git LFS. If you clone the repository and want to use this model, make sure to have Git LFS installed on your system.

## Citation

If you use the models please cite the MACE-OFF23 paper:

```bib
@misc{kovacs2023maceoff23,
      title={MACE-OFF23: Transferable Machine Learning Force Fields for Organic Molecules}, 
      author={Dávid Péter Kovács and J. Harry Moore and Nicholas J. Browning and Ilyes Batatia and Joshua T. Horton and Venkat Kapil and William C. Witt and Ioan-Bogdan Magdău and Daniel J. Cole and Gábor Csányi},
      year={2023},
      eprint={2312.15211},
      archivePrefix={arXiv},
}
```

and the FeNNol paper:

```bib
@article{ple2024fennol,
  title={FeNNol: an Efficient and Flexible Library for Building Force-field-enhanced Neural Network Potentials},
  author={Pl{\'e}, Thomas and Adjoua, Olivier and Lagard{\`e}re, Louis and Piquemal, Jean-Philip},
  journal={arXiv preprint arXiv:2405.01491},
  year={2024}
}
```

## Licence
By Downloading the MACE-OFF23 models you agree to the Academic Software License. This means you are free to use them for academic purpose, but not for commercial purposes. For details see `LICENSE.md` in this folder.

## Manually converting the models
To manually convert the MACE-MP models from the MACE library, use the provided `convert_mace_off_*.ipynb` notebooks. The notebooks use the `mace` library to load the models and the `fennol` library to save the models in the `.fnx` format. Both libraries must be installed in the same environment to run the notebook.
