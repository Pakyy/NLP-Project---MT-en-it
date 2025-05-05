# Exploring Translation Models: A Comparative Study of Seq2Seq and LLM Architectures for English-Italian Machine Translation

This repository contains the code and resources for a study comparing different neural network architectures for English-Italian machine translation. The primary goal of the project is to evaluate the performance of Sequence-to-Sequence (Seq2Seq) models and Large Language Models (LLMs) under various training paradigms.

## Project Description

The project investigates the following:

* Performance of models pre-trained on MT-specific tasks compared to those pre-trained on general tasks.
* The potential of training Seq2Seq models from scratch.
* The effectiveness of fine-tuning pre-trained LLMs using Low-Rank Adaptation (LoRA).
* Comparison of non-pre-trained LLMs to their pre-trained counterparts.

## Key Research Questions

* How do models pre-trained for MT-specific tasks perform relative to general-purpose pre-trained models on translation tasks?
* Can training Seq2Seq models from scratch achieve competitive performance, particularly when architectural capacity is increased?
* Does fine-tuning pre-trained LLMs with LoRA improve MT performance significantly?
* How do non-pre-trained LLMs compare to their pre-trained counterparts in terms of translation quality?

## Dataset

The TED2013 corpus, a parallel dataset of TED talk subtitles, is used for this study. The focus is specifically on the English-Italian subset.

* **Source Language:** English
* **Target Language:** Italian
* **Total Sentences:** 159,391
* **Source Language Tokens (English):** 2,670,718
* **Target Language Tokens (Italian):** 2,508,941

## Models

The following models are included in this study:

* **Seq2Seq Models:**
    * Pre-trained on Machine Translation Tasks (Helsinki-NLP OPUS-MT)
    * Pre-trained on General Tasks (T5-small)
    * Non-Pre-trained Seq2Seq Model
    * Non-Pre-trained Seq2Seq Model (Increased Dimensionality)
* **Large Language Models (LLMs):**
    * Pre-trained LLM (LLama-3.2-1B-Instruct)
    * Non-pre-trained LLMs

## Code and Resources

The repository provides:

* Code for data preprocessing, model training, and evaluation.
* Detailed analysis of the experimental results.
* Instructions for replicating the experiments.

## Results

The report includes both quantitative (ROUGE-L, BLEU, COMET scores) and qualitative analyses of the translation outputs. Key findings are:

* Pre-trained models generally outperform non-pre-trained models.
* Fine-tuning is crucial for adapting general-purpose pre-trained models to machine translation.
* LLMs show promise but require careful training and fine-tuning.

## Conclusion

This study provides a comprehensive comparison of Seq2Seq and LLM architectures for English-Italian machine translation. The findings highlight the importance of pre-training, fine-tuning, and model architecture in achieving high-quality translation.

## Future Work

* Combining pre-trained LLMs with targeted fine-tuning (e.g., LoRA).
* Expanding the dataset.
* Exploring hybrid approaches that integrate Seq2Seq and LLM models.
* Include the inverse translation task from Italian to English.
