# Homework project for MATH6450F


## Requirements and Usage 

### Requirements

- Python (**>=3.6**)
- PyTorch (**>=1.1.0**)
- Tensorboard(**>=1.4.0**) (for ***visualization***)
- Other dependencies (pyyaml, easydict)

PS: for TensorboardX version, check  tag [pt1.0](https://github.com/BIGBALLON/CIFAR-ZOO/releases/tag/pt1.0)


```bash
pip install -r requirements.txt
```

### Usage 

simply run the cmd for the training:

```bash
## GPUs for densenet100bc
CUDA_VISIBLE_DEVICES=0,1,2,3 python -u train.py --work-path ./experiments/cifar10/densenet100bc
``` 

We use yaml file ``config.yaml`` to save the parameters, check any files in `./experimets` for more details.  
You can see the training curve via tensorboard, ``tensorboard --logdir path-to-event --port your-port``.  
The training log will be dumped via logging, check ``log.txt`` in your work path.


## Acknowledgments

The code is adapted from CIFAR-ZOO: PyTorch implementation of CNNs for CIFAR dataset.

