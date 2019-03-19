# Conan Reborn
Diego: Data IntElliGence Out. Sprite Come from [Fast.ai](https://github.com/fastai/fastai).

# 模块结构

## core
`core` 模块封装了所有通用模块，包括通用接口和通用数据结构。类似`sklearn.classifiermixin`.
`sklearn_core`是和sklearn交互的核心接口，应该包含以下接口：

- data 类，封装一切从sklearn进和出的数据结构。可以和`sklearn.datasets`互通
- layers, 能够进行图层定义、dag图、或者pipeline的定义
- metrics，封装各类指标。

## train
用于组装数据、模型、损失函数、优化方法等。
定义：

```python
class Learner():
    "Trainer for `model` using `data` to minimize `loss_func` with optimizer `opt_func`."

class Recorder(LearnerCallback):
    "A `LearnerCallback` that records epoch, loss, opt and metric data during training."

class Estimator():
    "A estimator to evaulate learner.  "

```

# installation


# issues


# updates
