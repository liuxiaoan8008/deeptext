# bilstm-crf sequence labeling model

## Quick Start: Demo

[install](#install) deeptext and train your sequence labeling model to start sequence labeling!

Run command below to train a model:
```bash
python deeptext/run.py -m train -o your/model_dir -d you/train_data_file -v your/valid_data_file`
```

Run command below to test your model:
```bash
python deeptext/run.py -m test -o your/model_dir -d you/test_data_file`
```

Run command below to drop into an interactive session. For each sentence, model will return the sequence labeling result string.
```bash
python deeptext/run.py -m try -o your/model_dir`
```

<h2 id="install">install Deeptext</h2>

_Setting up Deeptext is easy!_

Deeptext requires Linux/OSX and Python 2.7. Its other dependencies are listed in requirements.txt. CUDA is strongly recommended for speed, but not necessary.

Run the following commands to clone the repository and install Deeptext:

```bash
git clone https://github.com/liuxiaoan8008/deeptext.git
cd deeptext; pip install -r requirements.txt; python setup.py develop
```

## training options
Optional arguments:
```
  -s    STEP,        train step, default is 500
  -b    BATCH,    train data's batch size, default is 256
  -l     LEN,          max document len, default is 25
  -e    EMBED,     word2vec embedding size, default is 100
  -p    PROB,       dropout prob, default is 0.5
```
