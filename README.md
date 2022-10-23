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

### Models:
For Hindi and Gujarati

* [IndicBART](https://huggingface.co/ai4bharat/IndicBART)
* [mT5](https://huggingface.co/google/mt5-base)
* [MBart](https://huggingface.co/facebook/mbart-large-50)
* [MBart + Adapters](https://docs.adapterhub.ml/classes/models/mbart.html)

For English

* [PEGASUS](https://huggingface.co/google/pegasus-large?text=The+tower+is+324+metres+%281%2C063+ft%29+tall%2C+about+the+same+height+as+an+81-storey+building%2C+and+the+tallest+structure+in+Paris.+Its+base+is+square%2C+measuring+125+metres+%28410+ft%29+on+each+side.+During+its+construction%2C+the+Eiffel+Tower+surpassed+the+Washington+Monument+to+become+the+tallest+man-made+structure+in+the+world%2C+a+title+it+held+for+41+years+until+the+Chrysler+Building+in+New+York+City+was+finished+in+1930.+It+was+the+first+structure+to+reach+a+height+of+300+metres.+Due+to+the+addition+of+a+broadcasting+aerial+at+the+top+of+the+tower+in+1957%2C+it+is+now+taller+than+the+Chrysler+Building+by+5.2+metres+%2817+ft%29.+Excluding+transmitters%2C+the+Eiffel+Tower+is+the+second+tallest+free-standing+structure+in+France+after+the+Millau+Viaduct.)
* [T5](https://huggingface.co/t5-large?text=My+name+is+Wolfgang+and+I+live+in+Berlin)
* [BART](https://huggingface.co/facebook/bart-large)
* [BRIO](https://huggingface.co/Yale-LILY/brio-cnndm-uncased)
* [ProphetNet](https://huggingface.co/microsoft/prophetnet-large-uncased)

### Run the script

To fine-tune any huggingface model you can use the `run.sh` script. When running the different models described in the paper, ensure you pass the appropriate arguments.

```sh
sh run.sh
```

