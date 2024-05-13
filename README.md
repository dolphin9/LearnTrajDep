## Learning Trajectory Dependencies for Human Motion Prediction
This is the code is forked from [LearnTrajDep](https://github.com/wei-mao-2019/LearnTrajDep)

Wei Mao, Miaomiao Liu, Mathieu Salzmann, Hongdong Li. 
[_Learning Trajectory Dependencies for Human Motion Prediction_](https://arxiv.org/abs/1908.05436). In ICCV 19.

### Dependencies

* cuda 12.4.1
* Python 3.10.14
* Pytorch 12.4.1
* [progress 1.5](https://pypi.org/project/progress/)

### Get the data
[3DPW](https://virtualhumans.mpi-inf.mpg.de/3DPW/) from their official website.

[Moyo](https://github.com/sha2nkt/moyo_toolkit) from github repo

### Mix dataset 3DPW and Moyo

open convert.ipynb and run all cells


### Training commands
All the running args are defined in [opt.py](utils/opt.py). We use following commands to train on different datasets and representations.
To train on angle space,
```bash
python main_3dpw.py --data_dir_3dpw "./dataset/mixed" --input_n 10 --output_n 30 --dct_n 40 --exp './log'
```
