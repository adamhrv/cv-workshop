# Computer Vision Workshop

## Setup

The basic steps are:

- clone project
- install miniconda
- create conda or pip environment and install dependencies
- run demos

### Clone Project

- `git clone https://github.com/adamhrv/cv-workshop`
- you may need to [install git first](https://gist.github.com/derhuerst/1b15ff4652a867391f03)

### Install Miniconda

- Try installing conda navigator via https://www.anaconda.com/products/individual
- Or download the installer file for your system <https://docs.conda.io/en/latest/miniconda.html>
- and then open terminal and run `bash Miniconda3-latest-MacOSX-x86_64.sh.sh` change this to the name of your .sh file first


### Create Conda Environemnt
- open terminal and `cd` into `cv-workshop`
```
conda create -n cv-workshop python=3.7
#conda activate cv-workshop  # to activate environment
conda install nb_conda
conda install -c conda-forge nb_conda_kernels
pip install -r requirements.txt
jupyter notebook
```

### YOLOV5
- to setup YOLOV5, initialize the submodule `git submodule init` and then `git submodule update`

### Troubleshooting

- dlib is only needed for the facial landmarking example. you can skip it if it's difficult to install. Building dlib may take a while. You may need to install or upgrade gcc or cmake. If on MacOS, you may also need to install xcode developer tools first. If issues, check <https://github.com/davisking/dlib/>
- conda: if you're using bash or zsh you may need to edit the conda env paths in your `~/.bashrc` or `~/.zshrc` file