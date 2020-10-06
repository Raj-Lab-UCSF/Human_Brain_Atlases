Human Brain Atlases Datalad Dataset
---

Datalad dataset containing collection of human brain parcellations. Please check and save your changes (`datalad status` and `datalad save`) if you make any chances in this directory. Refer to the [datalad handbook](http://handbook.datalad.org/en/latest/) before editing any directories. 

Currently this dataset contains:

    - AAL2
    - Brainnectome 246 regions
    - Desikan-Killiany 86 regions

Each of the above atlases are recorded as individual nested subdatasets according to datalad's workflows.

The origin of this dataset is `RAD-4BUJGH6-LT`, the lab's Mac laptop, created by Xihe Xie. This dataset has the following siblings:
     - `sachin`: [ssh://sachin/media/rajlab/DATASETS/Human_Brain_Atlases/brainnectome (git)]

#### Notes
 - `aal` contains only AAL2 right now, AAL3 has been released but has not been added to this dataset. Someone also needs to create and validate a LUT file if you want to use this atlas as an template. (Looking for help)
 - `desikan-killiany` contains a modified Freesurfer parcellation provided by Sneha Pandya. Please use carefully, be especially careful of your region ordering. 