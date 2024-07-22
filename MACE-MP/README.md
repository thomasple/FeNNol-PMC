# MACE-MP models

This folder contains the MACE-MP pre-trained foundation models for materials chemistry, parameterised for 89 chemical elements from 

    I. Batatia et al., A foundation model for atomistic materials chemistry, arXiv:2401.00096 (2023) 

https://doi.org/10.48550/arXiv.2401.00096

These models come in three sizes:
 - small --> `mace_mp_small.fnx`
 - medium --> `mace_mp_medium.fnx`
 - large --> `mace_mp_large.fnx`

All the models have been converted to `.fnx` format from the corresponding pytorch models provided in the [MACE repository](https://github.com/ACEsuit/mace) and the [MACE-MP repository](https://github.com/ACEsuit/mace-mp).

*Warning*: the file `mace_mp_large.fnx` is stored using Git LFS. If you clone the repository and want to use this model, make sure to have Git LFS installed on your system.

## Citation

If you use the models please cite the MACE-MP paper:

```bib
@article{batatia2023foundation,
      title={A foundation model for atomistic materials chemistry},
      author={Ilyes Batatia and Philipp Benner and Yuan Chiang and Alin M. Elena and Dávid P. Kovács and Janosh Riebesell and Xavier R. Advincula and Mark Asta and William J. Baldwin and Noam Bernstein and Arghya Bhowmik and Samuel M. Blau and Vlad Cărare and James P. Darby and Sandip De and Flaviano Della Pia and Volker L. Deringer and Rokas Elijošius and Zakariya El-Machachi and Edvin Fako and Andrea C. Ferrari and Annalena Genreith-Schriever and Janine George and Rhys E. A. Goodall and Clare P. Grey and Shuang Han and Will Handley and Hendrik H. Heenen and Kersti Hermansson and Christian Holm and Jad Jaafar and Stephan Hofmann and Konstantin S. Jakob and Hyunwook Jung and Venkat Kapil and Aaron D. Kaplan and Nima Karimitari and Namu Kroupa and Jolla Kullgren and Matthew C. Kuner and Domantas Kuryla and Guoda Liepuoniute and Johannes T. Margraf and Ioan-Bogdan Magdău and Angelos Michaelides and J. Harry Moore and Aakash A. Naik and Samuel P. Niblett and Sam Walton Norwood and Niamh O'Neill and Christoph Ortner and Kristin A. Persson and Karsten Reuter and Andrew S. Rosen and Lars L. Schaaf and Christoph Schran and Eric Sivonxay and Tamás K. Stenczel and Viktor Svahn and Christopher Sutton and Cas van der Oord and Eszter Varga-Umbrich and Tejs Vegge and Martin Vondrák and Yangshuai Wang and William C. Witt and Fabian Zills and Gábor Csányi},
      year={2023},
      eprint={2401.00096},
      archivePrefix={arXiv},
      primaryClass={physics.chem-ph}
}
```
```
MACE-Universal by Yuan Chiang, 2023, Hugging Face, Revision e5ebd9b, DOI: 10.57967/hf/1202, URL: https://huggingface.co/cyrusyc/mace-universal
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
The MACE-MP models are distributed under the MIT licence. See the `LICENCE` file in this folder for more information.

## Manually converting the models
To manually convert the MACE-MP models from the MACE library, use the provided `convert_mace_mp_*.ipynb` notebooks. The notebooks use the `mace` library to load the models and the `fennol` library to save the models in the `.fnx` format. Both libraries must be installed in the same environment to run the notebook.