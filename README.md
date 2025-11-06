# qiskit-slurm-template
A template and tutorial for submitting Qiskit jobs from an HPC cluster (e.g., via SLURM) using Python and conda environments, targeting the IBM Quantum runtime.

This repository provides example code, a submission script, and instructions for setting up a conda-environment based workflow for GPU/CPU HPC job submission of quantum jobs using Qiskit.

Contents
- __submission.sh__ — A sample SLURM submission script.
- __test1.py__ — Example Python job script demonstrating usage of Qiskit and the IBM Quantum runtime (via ibm-runtime and job submission). This is based of the Hellow World tutorial by <a href="https://quantum.cloud.ibm.com/docs/en/tutorials/hello-world">IBM Quantum</a>

Procedure: 
1. Before submitting the __submission.sh__ file it is important to have created a conda environment with all necessary dependencies. At our cliuster these are the steps which can be found in our <a href=https://docs.rcc.fsu.edu/software/conda/">docs</a>:
```
module load anaconda
conda create -n quantum
conda activate quantum
conda install conda-forge::qiskit-ibm-runtime
conda install conda-forge::qiskit
```
2. After this has been completed you should fill out your credentials on the __test1.py__ file and run the following command to run your job:
```
sbatch submission.sh
```
_Notes:_
- This was created by Florida State University's Research Computing Center therefore SLURM arguments and webproxy setup are particular for our cluster and should be edited for use in other HPC Centers
- This trial job should take anywhere from 7-15 seconds of your IBM Quantum time usage.
