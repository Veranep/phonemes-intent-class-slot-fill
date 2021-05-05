# phonemes-intent-class-slot-fill

## Contents
### clean_evaluation_data.org
Removes lines that failed to pass through the ASR error injection pipeline.
### evaluation.org
Contains a final processing of the evaluation data, including multiplying slot labels for words split into multiple words when turned into phonemes.
### evaluation_data.org
Contains an initial processing of the evaluation data.
### phoneme2vec_embeddings.org
The phoneme2vec embeddings using gensim's word2vec models are trained here.
### seq2seq_embeddings.org
The seq2seq embeddings using PyTorch are trained here.
### training_data.org
Contains an initial processing of the training data.

### Training data
The SQuAD and SUBJ training data used can be found [here](https://github.com/anjiefang/asr-error-robustness) and the CMU Pronouncing Dictionary data [here](http://www.speech.cs.cmu.edu/cgi-bin/cmudict/). The SQuAD and SUBJ training data can be downloaded using the [AWS Command Line Interface](https://docs.aws.amazon.com/cli/latest/userguide//aws-cli.pdf). Once downloaded, the `phoneme_embedding_training_set` needs to be placed under `./data`.
### Evaluation data
The evaluation data used can be found [here](https://github.com/MiuLab/SlotGated-SLU). Once downloaded, the `atis` and `snips` datasets also need to be placed under `./data`.
### Data Processing tools
The ASR errors in the evaluation data were created using this [ASR error injection pipeline](https://github.com/ailsamm/errorInjectionPipeline) and this [phonemizer](https://github.com/bootphon/phonemizer) was used to create phonemized versions of the text sequences that are in the datasets.
### Embeddings
Word2Vec skip-gram embeddings were trained using the [Gensim framework](https://radimrehurek.com/gensim/) and seq2seq models using [pytorch](https://pytorch.org/).
