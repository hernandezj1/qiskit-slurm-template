# qiskit-slurm-template
A template and tutorial for submitting Qiskit jobs from an HPC cluster (e.g., via SLURM) using Python and conda environments, targeting the IBM Quantum runtime.

This repository provides example code, a submission script, and instructions for setting up a conda-environment based workflow for GPU/CPU HPC job submission of quantum jobs using Qiskit.

Contents
- __submission.sh__ — A sample SLURM submission script.
- __test1.py__ — Example Python job script demonstrating usage of Qiskit and the IBM Quantum runtime (via ibm-runtime and job submission). This is based of the Hellow World tutorial by <a href="https://quantum.cloud.ibm.com/docs/en/tutorials/hello-world">IBM Quantum</a>

_Note:_
This was created by Florida State University's Research Computing Center therefore SLURM arguments and webproxy setup are particular for our cluster and should be edited for use in other HPC Centers
