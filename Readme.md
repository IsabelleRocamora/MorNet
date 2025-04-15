## MorNet

Implementation of the code accompanying the articleIsabelle Rocamora, Dino Ienco and Matthieu Ferry (31 Jan 2024) : Multisource deeplearning approach for automatic geomorphological mapping : the case of glacial moraines, Geo-spatial Information Science, https://doi.org/10.1080/10095020.2023.2292587.

**1. Prérequis**
- Python version 3.9.7
- Tensorflow version 2.7.0
- Rasterio version 1.2.10
- Numpy version 1.21.4
- scikit-learn 1.0.1


**2. Folder contents**

Subfolder :
- modules: which contains all the python code called by the main main.py code.

Four files :
 - main.py: to run the model and change the moraines assigned to each dataset (train, validation and test) under Linux
 - main_Windows.py: to run the model and change the moraines assigned to each dataset (train, validation and test) under Windows
 - Config.cfg: file to be filled in to define all parameters (number of filters, dropout rate, layer type, etc.)
 - methodo.docx: details of the various steps to be performed before launching the code



**3. Preprocess**

Folders to be created before launching the code:
- data folder: containing model input data, including ground truth (ROI_couche_positive.tif) and satellite data (see dictionaries in parameters.py), path to be specified in Config.cfg
- results folder: path to be specified in Config.cfg


**4. Linux launch command**

python main.py Config.cfg


**5. Script launch on Windows**

main_Windows.py
