# PanDerm
A General-Purpose Multimodal Foundation Model for Dermatology


## Installation
First clone the repo and cd into the directory:
```shell
git clone https://github.com/SiyuanYan1/PanDerm
cd PanDerm
```
Then create a conda env and install the dependencies:
```shell
conda create -n PanDerm python=3.10 -y
conda activate PanDerm
pip install torch==2.4.1 torchvision==0.19.1 torchaudio==2.4.1 --index-url https://download.pytorch.org/whl/cu118
pip install -r requirements.txt
```

## 1. Download PanDerm Pre-trained Weights

### Obtaining the Model Weights
Download the pre-trained model weights from [this Google Drive link](https://drive.google.com/file/d/1XHKRk2p-dS1PFQE-xRbOM3yx47i3bXmi/view?usp=sharing).

### Configuring the Model Path
After downloading, you need to update the model weights path in the code:

1. Open the file `PanDerm/LP_Eval/models/builder.py`
2. Locate line 42
3. Replace the existing path with the directory where you saved the model weights:

```python
root_path = '/path/to/your/PanDerm/Model_Weights/'
```
## 2. Organise your data into this directory (Public datasets used in this study can be downloaded here)

### Data split
| Dataset | Download Link 1 |   Download Link 2 |
| ------------- | ------------------ |------------------ |
| APTOS2019 | [Google Drive](https://drive.google.com/file/d/162YPf4OhMVxj9TrQH0GnJv0n7z7gJWpj/view?usp=sharing) |
| MESSIDOR2 | [Google Drive](https://drive.google.com/file/d/1vOLBUK9xdzNV8eVkRjVdNrRwhPfaOmda/view?usp=sharing)       
| IDRID | [Google Drive](https://drive.google.com/file/d/1c6zexA705z-ANEBNXJOBsk6uCvRnzmr3/view?usp=sharing)       
| PAPILA | [Google Drive](https://drive.google.com/file/d/1JltYs7WRWEU0yyki1CQw5-10HEbqCMBE/view?usp=sharing)      
| Glaucoma_fundus | [Google Drive](https://drive.google.com/file/d/18vSazOYDsUGdZ64gGkTg3E6jiNtcrUrI/view?usp=sharing)       
| JSIEC | [Google Drive](https://drive.google.com/file/d/1q0GFQb-dYwzIx8AwlaFZenUJItix4s8z/view?usp=sharing)       
| Retina | [Google Drive](https://drive.google.com/file/d/1vdmjMRDoUm9yk83HMArLiPcLDk_dm92Q/view?usp=sharing)     
| OCTID | [Google Drive](https://drive.google.com/file/d/1I7nAvbkJG4UF29J3HcyIW53rVEFcKRgm/view?usp=sharing)       




