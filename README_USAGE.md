# Usage

## Install dependencies

```bash
git clone https://github.com/egorsmkv/ocotillo-uk
cd ocotillo-uk

pipenv install
pipenv shell
```

## Run `transcribe.py`

```bash
# extend PYTHONPATH
export PYTHONPATH=`pwd`:$PYTHONPATH

# create a folder for traced version of the model
mkdir ocotillo/torchscript

# check that it works
python ocotillo/transcribe.py --path data/short

# if you like, you can run recognition without torchscript
python ocotillo/transcribe_no_traced.py --path data/short
```
