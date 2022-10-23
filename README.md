# Indian-Language-Summarization
This repository shows the implemenation of summarization models for Indian languages. The code and data available in the repo.

We use a modified fork of [huggingface transformers](https://github.com/huggingface/transformers) for our experiments.

### Creating environment
If you are using conda use the following command: 

```
conda env create -f environment.yml
```
Otherwise, for creating python environment use:

```
pip install requirements.txt
```

### Data format:

* We used the dataset released in the [ILSUM](https://ilsum.github.io/ilsum/2022/dataset.html) shared task

* Make sure to create `train, dev, test' csv files with column names "text" and "summary"


### Run the script

To fine-tune any huggingface model you can use the `run.sh` script. When running the different models described in the paper, ensure you pass the appropriate arguments.

```sh
sh run.sh
```

