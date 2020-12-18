# Fine-tuning Process.

This repository is about fine-tuning a pre-trained model using a annotated json file.
#Fine-Tuning

- Download the **Training json file** from the link.

https://git.openrainbow.org/cpaas-projects/qa-internip/-/tree/master/Haystack_input_files/Training%20(Fine-Tuning)\

- For reference, consult the Haystack Tutorial - 

https://github.com/deepset-ai/haystack/blob/master/tutorials/Tutorial2_Finetune_a_model_on_your_data.ipynb

## Notebooks

- **Finetuning_BERT_large_uncased.ipynb** - This notebook is about **Fine-Tuning** the pre-trained model - **bert-large-cased-whole-word-masking-finetuned-squad** .



- **Finetuning_minilm.ipynb** - This notebook is about **Fine-Tuning** the pre-trained model - **deepset/minilm-uncased-squad2** .


- **Finetuning_roBERTa_base_squad2.ipynb** - This notebook is about **Fine-Tuning** the pre-trained model - **deepset/roberta-base-squad2** .


## Recommendations

1. Implement **Fine-Tuning** on **Colab** (with **GPU**).
2. Move the **Fine-tuned model** once generatein Colab to your **Drive**, so that one can reuse it for **Evaluation** and also for **FastAPI Integration**.
3. One can implement **Fine-Tuning** on **Amazon Web Service**, once model is built, transfer it your local PC using **Win-SCP**.

## Parameters of Fine-Tuning in a Reader.

1. **n_epochs**: Number of iterations on the whole training data set. (I have n_epochs = 2)

2. **learning_rate**: Learning rate of the optimizer. (10^-5 by default)

3. **save_dir**: Path to store the final model.

4. **use_gpu**: Whether to use GPU (keep use_gpu = True if you are on Colab/AWS).

5. **num_processes**: The number of processes for multiprocessing'. Set to value of 1 to disable multiprocessing. Set to None to use all CPU cores minus one.


