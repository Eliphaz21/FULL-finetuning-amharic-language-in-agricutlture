# 🌾 Amharic LLM Fine-Tuning Pipeline for Agriculture

A complete end-to-end notebook for fine-tuning open-source Large Language Models on Amharic agricultural datasets using QLoRA and Unsloth.

This notebook is designed for researchers, students, startups, and developers who want to build high-quality Amharic AI assistants without creating an entire training pipeline from scratch.

Simply prepare your dataset, run the notebook, and deploy your model.

---

# ✨ Features

✅ Google Sheets dataset loading

✅ Amharic text cleaning and normalization

✅ Dataset quality validation

✅ Duplicate detection and removal

✅ Tokenizer fertility analysis

✅ Automatic train/validation/test splitting

✅ ChatML formatting

✅ QLoRA fine-tuning

✅ Training monitoring

✅ Automated evaluation

✅ GGUF export

✅ Hugging Face deployment

✅ Ollama deployment

---

#  Who Is This For?

This notebook is useful for anyone who wants to fine-tune a model on Amharic data, including:

* Agriculture chatbots
* Healthcare assistants
* Educational tutors
* Customer support agents
* Domain-specific AI assistants
* General Amharic instruction models

The notebook is domain-independent.

Simply replace the dataset with your own Amharic data.

---

# 🛠️ Technologies Used

* Python
* Unsloth
* Transformers
* TRL
* PEFT
* BitsAndBytes
* Hugging Face
* Datasets
* Pandas
* Google Colab

---

# 📊 Dataset Requirements

The notebook expects instruction-style data.

Example:

```json
{
  "user": "የስንዴ ተባይ እንዴት ማስቆጣጠር እችላለሁ?",
  "assistant": "የስንዴ ተባይን ለመቆጣጠር..."
}
```

Minimum recommended size:

* 5,000+ examples

Good quality:

* 20,000+ examples

Excellent quality:

* 50,000+ examples

---

#  Complete Workflow

## Step 1: Prepare Your Dataset

Collect high-quality Amharic question-answer pairs.

Examples:

* User → Assistant conversations
* FAQ datasets
* Expert responses
* Knowledge-base content

---

## Step 2: Upload Data

Upload your dataset to:

* Google Sheets
* CSV
* JSON

The notebook loads the data automatically.

---

## Step 3: Data Validation

The notebook checks:

* Missing values
* Empty responses
* Duplicate records
* Extremely short answers
* Dataset consistency

---

## Step 4: Data Cleaning

The notebook automatically:

* Fixes Unicode issues
* Normalizes Amharic text
* Removes duplicate records
* Cleans malformed examples

---

## Step 5: Dataset Quality Analysis

The notebook generates statistics such as:

* Dataset size
* Average response length
* Token counts
* Quality scores
* Train/Validation/Test distributions

---

## Step 6: Tokenizer Analysis

Before training, the notebook evaluates how efficiently the tokenizer handles Amharic text.

This helps identify tokenization bottlenecks that may affect model performance.

---

## Step 7: Convert to Chat Format

The dataset is transformed into instruction-tuning format.

Example:

```text
User: የቲማቲም ተክል ለምን ይደርቃል?

Assistant: የቲማቲም ተክል ሊደርቅ የሚችለው...
```

---

## Step 8: Fine-Tune the Model

The notebook uses:

* QLoRA
* 4-bit quantization
* LoRA adapters
* Gradient checkpointing

This allows efficient training even on Google Colab GPUs.

---

## Step 9: Evaluate the Model

The notebook automatically evaluates:

* Validation loss
* Sample generations
* Response quality
* Domain relevance

You can compare outputs before and after fine-tuning.

---

## Step 10: Save the Model

After training, the notebook saves:

* LoRA adapters
* Merged model
* Quantized model

for future deployment.

---

## Step 11: Push to Hugging Face

The notebook supports uploading directly to Hugging Face Hub.

After training:

```python
model.push_to_hub("your-model-name")
tokenizer.push_to_hub("your-model-name")
```

Your model becomes available for inference immediately.

---

## Step 12: Export GGUF

Generate GGUF files for:

* Ollama
* LM Studio
* Open WebUI
* Local inference

This allows running the model on consumer hardware.

---

# 📈 Expected Results

Results depend on:

* Dataset quality
* Dataset size
* Domain complexity

Generally:

* Better answers in Amharic
* Improved domain knowledge
* Better instruction following
* Reduced hallucinations

---

# 🔥 Example Use Cases

* Agricultural advisory chatbot
* Medical assistant
* Educational tutor
* Legal information assistant
* Business support chatbot
* Customer service assistant
* Government services assistant

---

# 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

Feel free to open issues, submit pull requests, or adapt the notebook for your own Amharic AI projects.

---

# 📜 License

This project is intended for educational, research, and production use.

Please verify the license of the selected base model before commercial deployment.

---
# 👨‍💻 Author: yeabsar andnet
Software Engineering Student | AI & Machine Learning Enthusiast

This notebook was created to make Amharic LLM fine-tuning more accessible for researchers, students, startups, and developers working on domain-specific AI systems.
If this notebook helps you build better Amharic AI systems, consider starring the repository and sharing it with the Amharic AI community.
