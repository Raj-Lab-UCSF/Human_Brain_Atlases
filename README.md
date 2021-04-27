Human Brain Atlases Datalad Dataset
---

Datalad dataset containing collection of human brain parcellations. Please check and save your changes (`datalad status` and `datalad save`) if you make any chances in this directory. Refer to the [datalad handbook](http://handbook.datalad.org/en/latest/) before editing any directories. 

Currently this dataset contains:

    - AAL2
    - Brainnectome 246 regions
    - Desikan-Killiany 86 regions
    - Glasser (HCP)

Each of the above atlases are recorded as individual nested subdatasets according to datalad's workflows.

The origin of this dataset is the lab's Mac laptop, created by Xihe Xie. This dataset has the following siblings:
     - `sachin`: [ssh://sachin/media/rajlab/DATASETS/Human_Brain_Atlases/ (git)]
     - `github`: [git@github.com:Raj-Lab-UCSF/Human_Brain_Atlases.git (git)]

### Cloning:
---
A DataLad dataset can be cloned by running

```
datalad clone <url>
```

Once a dataset is cloned, it is a light-weight directory on your local machine. At this point, it contains only small metadata and information on the identity of the files in the dataset, but not actual content of the (sometimes large) data files.

#### Retrieve dataset content

After cloning a dataset, you can retrieve file contents by running

```
datalad get <path/to/directory/or/file>
```

This command will trigger a download of the files, directories, or subdatasets you have specified.

DataLad datasets can contain other datasets, so called subdatasets. If you clone the top-level dataset, subdatasets do not yet contain metadata and information on the identity of files, but appear to be empty directories. In order to retrieve file availability metadata in subdatasets, run

```
datalad get -n <path/to/subdataset>
```

#### Notes
 - `aal` contains only AAL2 right now, AAL3 has been released but has not been added to this dataset. Someone also needs to create and validate a LUT file if you want to use this atlas as an template. (Looking for help)
 - `desikan-killiany` contains a modified Freesurfer parcellation provided by Sneha Pandya. Please use carefully, be especially careful of your region ordering. 
 - `glasser` contains a 256x256x256 grid file (`MMP_in_MNI_corr.nii.gz`) and a 182x218x182 grid file (`HCP-MMP_1mm.nii.gz`) both in 1mm resolution.
