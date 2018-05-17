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
- Please download the pre-trained model from [here](https://doc-0c-68-docs.googleusercontent.com/docs/securesc/g1920ikjrvli64f1ufo8k5nr6ekgjkvg/38o1dpjkf71upo0k3ap2434uf2v34q33/1526450400000/06583965992468288915/06583965992468288915/1Idhor57IAYsO7W4RDJDKbQ8VcsoABQo4?e=download&nonce=943nuh43fnvgg&user=06583965992468288915&hash=b1uhop7kkrsqkrqca7vnqj0mc8m7ioq6
) (google drive link), and put it under `./checkpoints/DDL-SR/`
- Test the model :
```bash
python test.py --dataroot datasets/ --name DDL-SR --phase test
```
The test results will be saved to here: `./results/DDL-SR/test_latest/images/output/`.

## Acknowledgments
This code borrows heavily from [pytorch-CycleGAN-and-pix2pix](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix).
