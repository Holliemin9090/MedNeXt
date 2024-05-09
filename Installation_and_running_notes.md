# Some installation and running notes
During installation, the nnunetv1 needs to be installed along with mednext:
(https://github.com/MIC-DKFZ/nnUNet/tree/nnunetv1)

When passing the environment variable, it should be:

export nnUNet_raw_data_base=/datasets/work/hb-breast-mri-dwt/work/breast_cancer_dwi_project/MedNeXt_venv/dataset/nnUNet_raw_data_base

export nnUNet_preprocessed=/datasets/work/hb-breast-mri-dwt/work/breast_cancer_dwi_project/MedNeXt_venv/dataset/nnUNet_preprocessed

export RESULTS_FOLDER=/datasets/work/hb-breast-mri-dwt/work/breast_cancer_dwi_project/MedNeXt_venv/dataset/nnUNet_results


In case the epoch number need to be changed, mednext/nnunet_mednext/training/network_training/network_trainer.py, line 97: self.max_num_epochs = 300#1000 
