# phonemes-intent-class
## Training data
The training data used can be found [here](https://github.com/anjiefang/asr-error-robustness). It can be downloaded using the [AWS Command Line Interface](https://docs.aws.amazon.com/cli/latest/userguide//aws-cli.pdf). Once downloaded, the `phoneme_embedding_training_set` needs to be placed under `./data`.
## Evaluation data
The evaluation data used can be found [here](https://github.com/MiuLab/SlotGated-SLU). Once downloaded, the `atis` and `snips` datasets also need to be placed under `./data`.
## Data Processing tools
The ASR errors were created using this [ASR error injection pipeline](https://github.com/ailsamm/errorInjectionPipeline) and this [phonemizer](https://github.com/bootphon/phonemizer) was used to create phonemized versions of the text sequences that are in the datasets.
