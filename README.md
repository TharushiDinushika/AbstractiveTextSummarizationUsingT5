# AbstractiveTextSummarizationUsingT5
## Overview:
### Install Dependencies: 
Install required packages: transformers, datasets, evaluate, and accelerate.

### Load and Clean the Dataset:
Loaded the CNN/DailyMail dataset.
Cleaned the text by lowercasing and removing unwanted characters (slashes, quotes, etc.).

### Preprocessing:
Tokenized the articles and summaries using a Hugging Face AutoTokenizer.
Added a "summarize: " prefix for the input.

### Train-Test Split:
Split the dataset into training (80%) and test (20%) sets.

### Model Training:
Used a pre-trained summarization model (e.g., BART) from Hugging Face.
Fine-tuned the model on the reduced dataset using Seq2SeqTrainer.

### Evaluation:
Evaluated the model using ROUGE scores.
Compared predicted and reference summaries for aggregated and unaggregated results.

### Model Saving:
Saved the fine-tuned model locally and pushed it to Hugging Face Hub.
