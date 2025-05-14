# Huggingface
The Hugging Face Hub is an open platform for sharing and discovering machine learning models, datasets, and demos. Think of it as GitHub, but specifically for ML assets like models, datasets, and training scripts.

| Feature               | Description                                                                                      |
| --------------------- | ------------------------------------------------------------------------------------------------ |
| **Model Hub**         | Thousands of pre-trained models for NLP, vision, audio, etc. (e.g., BERT, GPT, Stable Diffusion) |
| **Dataset Hub**       | Public datasets ready to use with the `datasets` library                                         |
| **Spaces**            | Host ML-powered web apps with Gradio or Streamlit                                                |
| **Versioning**        | Git-based version control and branches for models & datasets                                     |
| **Private Repos**     | Create private model/dataset repos for team or commercial use                                    |
| **CI/CD Integration** | Push from scripts, fine-tuning jobs, or CI pipelines                                             |
| **Community**         | Discussions, likes, downloads, model cards, and metrics                                          |


### pushing model to huggingfacehub
#### via python
```
from transformers import AutoModel, AutoTokenizer

model = AutoModel.from_pretrained("your_model_path")
model.push_to_hub("your-username/your-model-name")

tokenizer = AutoTokenizer.from_pretrained("your_model_path")
tokenizer.push_to_hub("your-username/your-model-name")
```

#### via cli
```
git lfs install
git clone https://huggingface.co/your-username/your-model
cd your-model
# Add files
git add .
git commit -m "Add model files"
git push
```


```
pip install huggingface_hub
huggingface-cli cache info
rm -rf ~/.cache/huggingface
du -sh ~/.cache/huggingface/transformers/* | sort -h      /*Show All Installed Models in Cache*/
```
