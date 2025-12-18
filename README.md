# Shallow seismic full waveform inversion with U net and a hybrid loss function(under review)
The paper will be published on Geophysical Journal International
This program aims to implement the simulate results for those researchers who are interested in our research. Significantly, this program only includes simulate data, while field data is limited to come out due to the privacy.

## Dataset
For the training process, we generate 6400 simulated velocity models and their seismograms by solving the elastic wave equation. The data can be found in 'MEUnet_Slurm/MEUnet/data'. 

## Training & Testing
### Pre-training
In our paper, 'MEUnet_Slurm' fold is implemented for training and testing. We have already placed the pre-trained model in the 'MEUnet_Slurm/MEUnet/models/SimulateModel'. Figure.5 in the paper can be implemented through running 'MEUnet_test.py'. Significantly, 'MEUnet_train_val.py' in 'MEUnet_Slurm' folder cannot be run due to the difference of Graphics Card Types. What we have mentioned in the paper is that we use four V100 for training at supercomputing center. But we also provide 'MEUnet' folder which can be run locally. Training code will take 20 minutes on 4 V100 and 3 hours on one Nvidia GTX4060.

### Transfer learning
The 'MEUnet_Transfer.py' in 'MEUnet_TransferLearning' fold can implement Figure.9 in the paper.

## Acknowledgements
This repository is based on the code from the following project:
- [FCNVMB-Deep-learning-based-seismic-velocity-model-building](https://github.com/YangFangShu/FCNVMB-Deep-learning-based-seismic-velocity-model-building?tab=readme-ov-file)
We thank the original authors for making their code publicly available.
