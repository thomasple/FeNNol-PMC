# ANI model family

This folder contains the ANI model family, which includes the following models:
- ANI-1X --> `ANI1X/ani1x_model*.fnx`
- ANI-1CCX --> `ANI1CCX/ani1ccx_model*.fnx`
- ANI-2X --> `ANI2X/ani2x_model*.fnx`

All the models have been converted to `.fnx` format from the corresponding pytorch models provided in the [TorchANI repository](https://github.com/aiqm/torchani) and the [ani-model-zoo](https://github.com/aiqm/ani-model-zoo).

## Model descriptions
Below are the model descriptions provided in TorchANI.
### ANI-1X
The ANI-1x model is an ensemble of 8 networks that was trained using active learning on the ANI-1x dataset, the target level of theory is wB97X/6-31G(d). It predicts energies on HCNO elements exclusively, it shouldn't be used with other atom types.

    - ani-1x_8x on GitHub:
        https://github.com/isayev/ASE_ANI/tree/master/ani_models/ani-1x_8x

    - Active Learning Paper:
        https://aip.scitation.org/doi/abs/10.1063/1.5023802

### ANI-1CCX
The ANI-1ccx model is an ensemble of 8 networks that was trained on the ANI-1ccx dataset, using transfer learning. The target accuracy is CCSD(T)*/CBS (CCSD(T) using the DPLNO-CCSD(T) method). It predicts energies on HCNO elements exclusively, it shouldn't be used with other atom types.

    - ani-1ccx_8x on GitHub:
        https://github.com/isayev/ASE_ANI/tree/master/ani_models/ani-1ccx_8x

    - Transfer Learning Paper:
        https://doi.org/10.26434/chemrxiv.6744440.v1

### ANI-2X
The ANI-2x model is an ensemble of 8 networks that was trained on the ANI-2x dataset. The target level of theory is wB97X/6-31G(d). It predicts energies on HCNOFSCl elements exclusively it shouldn't be used with other atom types.

    - ANI2x Results on GitHub:
        https://github.com/cdever01/ani-2x_results

    - ANI2x Paper:
        https://doi.org/10.26434/chemrxiv.11819268.v1



## Licence
The ANI models are distributed under the MIT licence. See the `LICENCE` file in this folder for more information.

## Manually converting the models
To manually convert the ANI models from the TorchANI library, use the provided `convert_ani.ipynb` notebook. The notebook uses the `torchani` library to load the models and the `fennol` library to save the models in the `.fnx` format. Both libraries must be installed in the same environment to run the notebook.