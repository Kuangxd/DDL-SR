# DDL-SR

Pytorch implementation of our method for stripe noise removal.

## Prerequisites
- Linux or macOS
- Python 2 or 3
- NVIDIA GPU + CUDA cuDNN

## Getting Started
### Installation
- Install PyTorch and dependencies from http://pytorch.org
- Install python libraries [dominate](https://github.com/Knio/dominate).
```bash
pip install dominate
```

### Testing
- A few example test images are included in the `datasets` folder.
- Please download the pre-trained model from [here](https://drive.google.com/drive/folders/1NdhrYDniB6flKJTnfzYcVFKdt2EBCaZR) (google drive link), and put it under `./checkpoints/DDL-SR/`
- Test the model :
```bash
python test.py --dataroot datasets/ --name DDL-SR --phase test
```
The test results will be saved to here: `./results/DDL-SR/test_latest/images/output/`.

## Acknowledgments
This code borrows heavily from [pytorch-CycleGAN-and-pix2pix](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix).
