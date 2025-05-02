🧠 T5 Text Summarization Using Transformers
This project explores the use of the T5 (Text-to-Text Transfer Transformer) model for the task of abstractive text summarization. It leverages transfer learning by fine-tuning the pre-trained t5-small model on a dataset of news articles, aiming to generate concise and coherent summaries from long input texts.

📌 Project Overview
Model Used: t5-small from Hugging Face Transformers.

Task: Abstractive summarization of news articles.

Approach: Fine-tune a pre-trained transformer model using supervised learning, then evaluate it using standard NLP metrics.

🔍 Methods and Techniques
1. Model Fine-Tuning
Pre-trained t5-small is fine-tuned on a summarization dataset.

Input format: "summarize: <article_text>"

Tokenization is handled by the T5 tokenizer with truncation and padding.

2. Evaluation Metrics
The model is evaluated using multiple metrics to capture different quality aspects:

ROUGE Scores (Recall-Oriented Understudy for Gisting Evaluation):

ROUGE-1: Overlap of unigrams.

ROUGE-2: Overlap of bigrams.

ROUGE-L: Longest common subsequence between reference and generated summary.

BERTScore:

Leverages contextual embeddings from BERT to compute similarity between predicted and reference summaries.

Focuses on semantic matching rather than exact n-gram overlap.

Length-Based Statistics:

Measures the average token length of inputs, predictions, and reference summaries to analyze compression quality.

Qualitative Examples:

Human-readable side-by-side comparisons of original text, reference summaries, and model predictions for interpretability.
