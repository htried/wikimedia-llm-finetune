# wikimedia-llm-finetune
A repository with code for finetuning open source LLMs on Wikimedia data.

Notebooks run on Google Colab Pro infrastructure using A100 (40GB) GPUs for training and V100 (16GB) for testing.

With 40GB of GPU RAM, you can finetune up to 12-13 blocks (out of 32 total blocks) of [MPT-7B](https://github.com/mosaicml/llm-foundry/).

With 16GB of GPU RAM, you can generate text using MPT-7B for testing outputs.

Code in this repository is inspired by of several existing LLM finetuning Github repos:
- [alpaca-lora](https://github.com/tloen/alpaca-lora) (for prompt construction / training procedure)
- [mpt_7b_fine_tuning](https://github.com/antecessor/mpt_7b_fine_tuning)
- [MPT-7B-Instruct Fine Tuning Tutorial](https://colab.research.google.com/drive/1DqKNPOzyMUXmJiJFvJITOahVDxCrA-wA) (model / tokenizer loading, output generation)

Datasets used in this repository:
- [htriedman/wiki-sparql](https://huggingface.co/datasets/htriedman/wiki-sparql)
- [htriedman/wikisql](https://huggingface.co/datasets/htriedman/wikisql)
