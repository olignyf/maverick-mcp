
## Install reddis
```bash
sudo apt install build-essential tcl curl
curl -O http://download.redis.io/redis-stable.tar.gz
tar xzf redis-stable.tar.gz
cd redis-stable
make
make test
sudo make install
```

## Install python libraries
```bash
source ~/venv/bin/activate
pip install uv
uv sync --dev --all-extras
uv add pandas pandas-ta ta-lib aiohttp python-dotenv numpy==1.26.4
```


## Test talib
```bash
python -c "import talib; print(talib.__version__)"
```
0.6.8

## Run

```bash
make dev
```

