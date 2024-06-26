# CT Body Composition

This repository provides code and models weights for training and running body composition estimation models on
abdominal CT scans.

### Note: Git-LFS

The model weights are stored in this repository using `git-lfs`. Please ensure you have git-lfs set up following
the instructions [here](https://git-lfs.com/) instructions before cloning the repository.

### Getting Started

After cloning the repository, you have two options for setting up the environment.
You may install all the necessary components directly on your system, or if you have docker on your machine,
you may build a docker image that contains all the necessary requirements.

See the documentation pages for further details:
* [Installation](docs/installation.md) - For installing directly on your system
* [Docker](docs/docker.md) - For building and using the docker image
* [Training](docs/training.md) - For training new models
* [Inference](docs/inference.md) - For running the model on new data

### Publications

This code accompanies the following publication:

> *Population-Scale CT-Based Body Composition Analysis Of a Large Outpatient Population Using Deep Learning To Derive
> Age, Sex, and Race-Specific Reference Curves*
>
> K. Magudia, C.P. Bridge, C.P. Bay, A. Babic, F.J. Fintelmann, F. Troschel, N. Miskin, W. Wrobel, L.K. Brais,
> K.P. Andriole, B.M. Wolpin, and M.H. Rosenthal
>
> *Radiology*
>
> [Article at RSNA](https://pubs.rsna.org/doi/10.1148/radiol.2020201640)

Furthermore, an earlier version of the same model was developed for the following publication:

> *Fully-Automated Analysis of Body Composition from CT in Cancer Patients Using Convolutional Neural Networks*
>
> C.P. Bridge, M. Rosenthal, B. Wright, G. Kotecha, F. Fintelmann, F. Troschel, N. Miskin, K. Desai, W. Wrobel,
> A. Babic, N. Khalaf, L. Brais, M. Welch, C. Zellers, N. Tenenholtz, M. Michalski, B. Wolpin, and K. Andriole
>
> Workshop on Clinical Image-based Procedures, MICCAI, Granada 2018
>
> [Article at Springer Link](https://link.springer.com/chapter/10.1007/978-3-030-01201-4_22),
> [Article at Arvix](https://arxiv.org/abs/1808.03844)

If you use this code in your publication, please cite these papers.

### Acknowledgements

The Python code for body composition estimation was written by Christopher Bridge at MGH & BWH Center for Clinical Data
Science (now [MGB AI](https://www.massgeneralbrigham.org/en/research-and-innovation/centers-and-programs/data-science))
and the [Athinoula A. Martinos Center for Biomedical Imaging](https://martinos.org), Alex Chowdhury, and Sahil
Nalawade both at the Department of Informatics & Analytics at the
[Dana Farber Cancer Institute](https://www.dana-farber.org/). The z-score curve fitting R code in the `stats` directory
was written by Camden Bay at Brigham and Women's Hospital. The project was conceived and led by Michael Rosenthal at
the Dana Farber Cancer Institute and Florian Fintelmann at Massaschusetts Department of Radiology with assistance
from Kirti Magudia at Brigham and Women's hospital.

- Chris Bridge, Massachusetts General Hospital (cbridge at mgh dot harvard dot edu)
- Alex Chowdhury, Dana Farber Cancer Institute (Alexander underscore Chowdhury at dfci dot harvard dot edu)
- Kirti Magudia, Duke University (kirti dot magudia at duke dot edu)
- Michael Rosenthal, Dana Farber Cancer Institute (Michael underscore Rosenthal at dfci dot harvard dot edu)
- Florian Fintelmann, Massachusetts General Hospital (fintelmann at mgh dot harvard dot edu)
- Camden Bay, Brigham and Women's Hospital (cpbay at bwh dot harvard dot edu)

### See Also

The z-score fitting process associated with this work is available
[here](https://github.com/Rosenthal-Lab-at-Dana-Farber/bodycomp-popref).
