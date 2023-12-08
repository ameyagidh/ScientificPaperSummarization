# Summarization

This project showcases an attempt to summarize and simplify scientific documents by fine tuning language models on custom preprocessed data

### Installation

#### Clone the repository: 

`git clone https://github.com/ameyagidh/ScientificPaperSummarization
.git`

#### Change to the project directory: 

`cd Summarization`

#### Install dependencies: 

`pip install -r requirements.txt`

#### Get Huggingface login

Generate hugginface token to use the pretrained models and datasets.

#### To generate a small sample of pre-processed data, follow these steps:

This will generate a JSON with 'topic', 'summary' and 4 preprocessed contents

`python data.py`

#### To use Summarization, follow these steps:

`python test.py -t "This is the input text for summarization." -m "Choose from list of models"`

#### To train Summarization, follow these steps:

This may not run, if you do not posses the sufficient cuda core and memory if you desire to run it on CPU change the `fp16=False` under Seq2SeqTrainingArgument.

`python train.py --dataset 3500_train_trad.json --model google/pegasus`

#### To evaluate the Summarization, follow these steps:

`python evaluation.py`

### Contributing follow these steps:

If you would like to contribute to Summarization, you can follow these steps:


Fork the repository.
Create a new branch for your contribution: 
`git checkout -b feature/your-feature-branch`

Make your changes and commit them: 
`git commit -m "Add your commit message here"`

Push your changes to your forked repository: 
`git push origin feature/your-feature-branch`

Create a pull request to the main repository, explaining your changes and their significance.

### Contact
For any questions, suggestions, or concerns, please feel free to contact the project maintainer at pawar.prath@northeastern.edu and sharan.a@northeastern.edu

We appreciate your interest and contributions to Summarization! Thank you for your support.


### Links to models and datasets

## Models

1. Pegasus 

2. Bartn


