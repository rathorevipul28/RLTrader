# RL for Bitcoin Trading

Data sets: https://www.cryptodatadownload.com/data/northamerican/

#installation, no CUDA installation needed

conda create --name rltrader python=3.6.8 pip git

conda activate rltrader

conda install tensorflow-gpu

git clone https://github.com/rathorevipul28/RLTrader

pip install -r RLTrader/requirements.txt

# Training and Testing

We just let the agent train and run with the default PPO2 hyper-parameters, available in `./data/params.db`. The `stable-baselines` library provides a great set of default parameters that work for most problem domains.

Help command - python ./cli.py --help

Sample command to train and save log to output file - python ./cli.py --input-data-path data/input/coinbase-1h-btc-usd.csv train > 1h_train.txt

Sample command to train and save log to output file - python ./cli.py --input-data-path data/input/coinbase-1h-btc-usd.csv test > 1h_test.txt 


