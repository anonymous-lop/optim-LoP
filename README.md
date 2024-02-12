
## Installation

Make sure to install CUDA 11 or higher properly.

```shell
pip3 install -U pip
python3 -m venv venv
source venv/bin/activate
pip3 install -r requirements.txt
```

After this, test the installation by running the following command:

```python
python3 -c "import torch; print(torch.cuda.is_available())"
```

If the output is `True`, then the installation is successful.

## Running
```python
CUDA_VISIBLE_DEVICES=0 python rainbow.py Alien-v5 Boxing-v5 Breakout-v5 --seed=42 --optimizer=cadam --beta0 0.5 --step-per-epoch=50000 --buffer-size=50000
```

