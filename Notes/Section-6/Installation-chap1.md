# Installation Chapitre 1

## Procédure Installation - Pytorch

Il est recommandé de créer un environnement Anaconda au préalable. Un environnement permet d'installer des modules spécifiquement au projet sur lequel au travail, afin d'éviter les conflits entre différentes versions. Par exemple, si vous avez aussi suivi le cours Deep Learning de A à Z, il est important de séparer les deux projets dans deux environnements différents.

Avant d'installer PyTorch

Lancer la commande create --name artificialintelligenceaz python=3.6 anaconda.
```
(base) C:\Users\mchettih>conda create --name artificialintelligenceaz python=3.6 anaconda
Solving environment: done

## Package Plan ##

  environment location: C:\Users\mchettih\AppData\Local\conda\conda\envs\artificialintelligenceaz

  added / updated specs:
    - anaconda
    - python=3.6


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    cffi-1.11.5                |   py36h74b6da3_1         213 KB
    ...
    ...
    ...
    lazy-object-proxy-1.3.1    |   py36hfa6e2cd_2          31 KB
    ------------------------------------------------------------
                                           Total:       491.2 MB

The following NEW packages will be INSTALLED:

    alabaster:                          0.7.12-py36_0
    ...
    ...
    ...
    zstd:                               1.3.7-h508b16e_0

Proceed ([y]/n)? y


Downloading and Extracting Packages
cffi-1.11.5          |  213 KB | ############################################################################## | 100%
...
...
...
lazy-object-proxy-1. |   31 KB | ############################################################################## | 100%
Preparing transaction: done
Verifying transaction: done
Executing transaction: done
#
# To activate this environment, use
#
#     $ conda activate artificialintelligenceaz
#
# To deactivate an active environment, use
#
#     $ conda deactivate
```

Lancer la command conda activate artificialintelligenceaz
```
(base) C:\Users\mchettih>conda activate artificialintelligenceaz

(artificialintelligenceaz) C:\Users\mchettih>
```

Lancer la commande conda install pytorch-cpu torchvision-cpu -c pytorch
```
(artificialintelligenceaz) C:\Users\mchettih>conda install pytorch-cpu torchvision-cpu -c pytorch
Solving environment: done

## Package Plan ##

  environment location: C:\Users\mchettih\AppData\Local\conda\conda\envs\artificialintelligenceaz

  added / updated specs:
    - pytorch-cpu
    - torchvision-cpu


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    pytorch-cpu-1.0.0          |      py3.6_cpu_1        56.6 MB  pytorch
    conda-4.6.3                |           py36_0         1.7 MB
    anaconda-custom            |   py36h363777c_0           9 KB
    ca-certificates-2019.1.23  |                0         158 KB
    torchvision-cpu-0.2.1      |             py_2          37 KB  pytorch
    ninja-1.8.2                |   py36he980bc4_1         110 KB
    ------------------------------------------------------------
                                           Total:        58.6 MB

The following NEW packages will be INSTALLED:

    ninja:           1.8.2-py36he980bc4_1
    pytorch-cpu:     1.0.0-py3.6_cpu_1    pytorch
    torchvision-cpu: 0.2.1-py_2           pytorch

The following packages will be UPDATED:

    anaconda:        2018.12-py36_0               --> custom-py36h363777c_0
    ca-certificates: 2018.03.07-0                 --> 2019.1.23-0
    conda:           4.5.12-py36_0                --> 4.6.3-py36_0

Proceed ([y]/n)? y


Downloading and Extracting Packages
pytorch-cpu-1.0.0    | 56.6 MB   | ############################################################################ | 100%
conda-4.6.3          | 1.7 MB    | ############################################################################ | 100%
anaconda-custom      | 9 KB      | ############################################################################ | 100%
ca-certificates-2019 | 158 KB    | ############################################################################ | 100%
torchvision-cpu-0.2. | 37 KB     | ############################################################################ | 100%
ninja-1.8.2          | 110 KB    | ############################################################################ | 100%
Preparing transaction: done
Verifying transaction: done
Executing transaction: done

(artificialintelligenceaz) C:\Users\mchettih>
```

Pour lancer spyder lancer la commande spyder apres avoir activer l'environnement 
```
conda activate artificialintelligenceaz
spyder
```

## Procédure Installation - Kivy

Executer dans "Anaconda Prompt" en tant que admin, les commande suivantes:
```
python -m pip install --upgrade pip wheel setuptools
python -m pip install docutils pygments pypiwin32 kivy.deps.sdl2 kivy.deps.glew
python -m pip install kivy.deps.gstreamer
python -m pip install kivy.deps.angle
python -m pip install kivy
python -m pip install pygame
```
