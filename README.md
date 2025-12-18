# Shallow seismic full waveform inversion with U net and a hybrid loss function(being organized)
The paper will be published on Geophysical Journal International
This program aims to reproduce the simulate results for those researchers who are interested in our research. Significantly, this program only includes simulate data, while field data is limited to come out due to the privacy.

## Training & Testing
### Pre-training
In our paper, 'MEUnet_Slurm' is implemented for training and testing. We have already placed the pre-trained model in the 'MEUnet_Slurm/MEUnet/models/SimulateModel'.  Figure. 5 in the paper can be implemented through running 'MEUnet_test.py'. Significantly, 'MEUnet_train_val.py' in 'MEUnet_Slurm' folder cannot be run due to the difference of Graphics Card Types. What we have mentioned in the paper is that we use four V100 for training at the school's supercomputing center. But we also provide 'MEUnet' folder which can be run locally.

### Transfer learning

