
# MMAction

全面支持视频动作分析的各种任务，包括动作识别（action recognition）、时域动作检测（temporal action detection）以及时空动作检测（spatial-temporal action detection）。

支持多种流行的数据集，包括 Kinetics、THUMOS、UCF101、ActivityNet、Something-Something、以及 AVA 等。

已实现多种动作分析算法框架，包括 TSN、I3D、SSN、以及新的 spatial-temporal action detection 方法。MMAction 还通过 Model Zoo 提供了多个预训练模型，以及它们在不同数据集上的性能指标。

采用高度模块化设计。用户可以根据需要对不同模块，比如 backbone 网络、采样方案等等进行灵活重组，以满足不同的应用需要。

## Introduction
MMAction is an open source toolbox for action understanding based on PyTorch.
It is a part of the [open-mmlab](https://github.com/open-mmlab) project developed by [Multimedia Laboratory, CUHK](http://mmlab.ie.cuhk.edu.hk/).

### Major Features
- MMAction is capable of dealing with all of the tasks below.

  - action recognition from trimmed videos
  - temporal action detection (also known as action localization) in untrimmed videos
  - spatial-temporal action detection in untrimmed videos. 
 

- Support for various datasets

  Video datasets have emerging throughout the recent years and have greatly fostered the devlopment of this field.
  MMAction provides tools to deal with various datasets.

- Support for multiple action understanding frameworks

  MMAction implements popular frameworks such as TSN, I3D for action recognition and SSN for temporal action detection.
  For the recently introduced spatial temporal atomic action detection, a Fast-RCNN baseline is provided.

- Modular design

  The tasks in human action understanding share some common aspects such as backbones, and long-term and short-term sampling schemes.
  Also, tasks can benefit from each other. For example, a better backbone for action recognition will bring performance gain for action detection. 
  Modular design enables us to view action understanding in a more integrated perspective.

## License
The project is release under the [Apache 2.0 license](https://github.com/open-mmlab/mmaction/blob/master/LICENSE).

## Updates

v0.1.0 (19/06/2019)
- MMAction is online!

## Model zoo
Results and reference models are available in the [model zoo](https://github.com/open-mmlab/mmaction/blob/master/MODEL_ZOO.md).

## Installation
Please refer to [INSTALL.md](https://github.com/open-mmlab/mmaction/blob/master/INSTALL.md) for installation.

Update: for Docker installation, Please refer to [DOCKER.md](https://github.com/open-mmlab/mmaction/blob/master/DOCKER.md) for using docker for this project.

## Data preparation
Please refer to [DATASET.md](https://github.com/open-mmlab/mmaction/blob/master/DATASET.md) for a general knowledge of data preparation.
Detailed documents for the supported datasets are available in `data_tools/`.

## Get started
Please refer to [GETTING_STARTED.md](https://github.com/open-mmlab/mmaction/blob/master/GETTING_STARTED.md) for detailed examples and abstract usage.

## Contributing
We appreciate all contributions to improve MMAction.
Please refer to [CONTRUBUTING.md](https://github.com/open-mmlab/mmaction/blob/master/CONTRIBUTING.md) for the contributing guideline.

## Citation
If you use our codebase or models in your research, please cite this work.
We will release a technical report later.
```
@misc{mmaction2019,
  author =       {Yue Zhao, Yuanjun Xiong, Dahua Lin},
  title =        {MMAction},
  howpublished = {\url{https://github.com/open-mmlab/mmaction}},
  year =         {2019}
}
```

## Contact
If you have any question, please file an issue or contact the author:
```
Yue Zhao: thuzhaoyue@gmail.com
```
