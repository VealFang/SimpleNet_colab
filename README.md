# SimpleNet

**SimpleNet: A Simple Network for Image Anomaly Detection and Localization**

*Zhikang Liu, Yiming Zhou, Yuansheng Xu, Zilei Wang**

Paper: [arxiv 2303.15140](https://arxiv.org/pdf/2303.15140.pdf)

##  Introduction

This repo  implemented **SimpleNet** with coalb and self-built dataset.

SimpleNet is a simple defect detection and localization network that built with a feature encoder, feature generator and defect discriminator. It is designed conceptionally simple without complex network deisng, training schemes or external data source.

## Get Started 

### Environment 

- python3
- timm
- torch
- torchvision
- numpy
- opencv-python

### Data

Edit `config.txt` to edit dataset class and dataset path.

#### MvTecAD

Download the dataset from [here](https://www.mvtec.com/company/research/datasets/mvtec-ad/).

The dataset folders/files follow its original structure.

#### Or use your own data

step 1. keep the dataset folder structure same as MvTecAD

step 2. change _CLASSNAMES in `datasets/mvtec.py`

### Run

#### Colab preparation

1. download the repository: `!git clone https://github.com/VealFang/SimpleNet_colab.git`
2. download or upload dataset zipfile
3. unzip dataset: `!unzip dataset.zip`
4. change work path: `%cd SimpleNet_colab`

#### Train

```
python main.py < config.txt
```

## Citation
```
@misc{liu2023simplenet,
      title={SimpleNet: A Simple Network for Image Anomaly Detection and Localization}, 
      author={Zhikang Liu and Yiming Zhou and Yuansheng Xu and Zilei Wang},
      year={2023},
      eprint={2303.15140},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```

## License

All code within the repo is under [MIT license](https://mit-license.org/)
