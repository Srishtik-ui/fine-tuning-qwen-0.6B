# Fine-Tuning Qwen 0.6B using LoRA and Unsloth

This project demonstrates how to fine-tune the Qwen 0.6B Large Language Model (LLM) using parameter-efficient fine-tuning techniques such as LoRA (Low-Rank Adaptation) and the Unsloth framework. The notebook provides an end-to-end workflow, from loading the base model to training and inference. Qwen 0.6B is a lightweight language model that is commonly used for experimentation and custom task adaptation. :contentReference[oaicite:0]{index=0}

## 🚀 Features

- Load and configure the Qwen 0.6B model
- Efficient fine-tuning with LoRA
- Faster training using Unsloth
- Dataset preprocessing and tokenization
- Model training and evaluation
- Save and reload fine-tuned checkpoints
- Run inference on custom prompts
- Google Colab compatible

## 📂 Project Structure

```text
fine-tuning-qwen-0.6B/
│
├── QWEN_MODEL.ipynb      # Main training notebook
├── README.md             # Project documentation
└── requirements.txt      # Dependencies (optional)
🛠️ Technologies Used
Python
PyTorch
Transformers
PEFT (LoRA)
Unsloth
Hugging Face Datasets
Google Colab
📋 Prerequisites

Before running the notebook, ensure you have:

Python 3.10+
CUDA-enabled GPU (recommended)
Hugging Face account
Google Colab or Jupyter Notebook
📦 Installation

Clone the repository:

git clone https://github.com/Srishtik-ui/fine-tuning-qwen-0.6B.git
cd fine-tuning-qwen-0.6B

Install dependencies:

pip install -U transformers datasets accelerate peft trl unsloth
▶️ Running the Notebook
Open QWEN_MODEL.ipynb.
Install required packages.
Load the Qwen 0.6B base model.
Prepare the training dataset.
Configure LoRA parameters.
Train the model.
Save the fine-tuned model.
Run inference on custom prompts.
🧠 Fine-Tuning Workflow
Dataset
   ↓
Preprocessing
   ↓
Tokenization
   ↓
LoRA Configuration
   ↓
Model Training
   ↓
Evaluation
   ↓
Save Model
   ↓
Inference
📊 Training Configuration

Example configuration:

learning_rate = 2e-4
batch_size = 2
num_epochs = 3
lora_rank = 16
lora_alpha = 16

These values can be adjusted based on dataset size and GPU availability.

💡 Example Inference
prompt = "Explain machine learning in simple terms."

response = model.generate(...)
print(response)
Sample Output
Machine learning is a branch of artificial intelligence that allows computers to learn patterns from data and make predictions without being explicitly programmed.
📈 Applications
Chatbots
Question Answering Systems
Text Generation
Domain-Specific Assistants
Educational AI Tools
Research Projects
🤝 Contributing

Contributions are welcome.

Fork the repository
Create a feature branch
git checkout -b feature-name
Commit changes
git commit -m "Add new feature"
Push changes
git push origin feature-name
Open a Pull Request
👩‍💻 Author

Srishti Kumari

B.Tech Data Science Student
Machine Learning Enthusiast
AI & Data Analytics Learner

GitHub: https://github.com/Srishtik-ui

⭐ Support

If you found this project useful, please consider giving it a ⭐ on GitHub.

📜 License

This project is licensed under the MIT License.
