# 🚀 DeepSeek-14B Fine-Tuning Project
This project aims to fine-tune DeepSeek-R1-Distill-Qwen-14B using Zhihu and Xiaohongshu datasets separately. The fine-tuning is conducted using the LoRA method with the Unsloth framework, optimized for Colab + A100 with BF16 support. 

## 📁 Project Structure
```bash
DeepSeek-Finetune/
│── datasets/                        # Dataset folder (JSON data + preprocessing scripts)
│   ├── raw/                         
│   │   ├── zhihu_data_without_clean.json         
│   │   ├── xhs_data_without_clean.json            
│   ├── data/                         
│   │   ├── zhihu_data.json          
│   │   ├── xhs_data.json            
│   ├── preprocess_zhihu.py          
│   ├── preprocess_xhs.py    
│── models/                                         
│   ├──zhihu_colab_demo.ipynb            
│   ├──xhs_colab_demo.ipynb
│── checkpoints/                       
│   ├──zhihu_checkpoints            
│   ├──xhs_checkpoints
│── wandb/                       
│   ├──zhihu_train_loss.png           
│   ├──xhs_train_loss.png                   
│── requirements.txt                 
│── README.md                        
```

📚 Setup & Installation
### 1️⃣ Install dependencies
Run the following command to install required libraries:
```bash
pip install -r requirements.txt
```
Or manually install:
```
pip install unsloth transformers datasets huggingface_hub wandb
```
### 2️⃣Get Weights & Biases key
```bash
import wandb
wb_token = "xxx"
wandb.login(key=wb_token)
run = wandb.init(
    project='fine_tune_deepseek',
    job_type="training",
    anonymous="allow"
)
```
### 3️⃣Get Hugging Face key
```bash
from huggingface_hub import login
hf_token = "xxx"
login(hf_token)
```
## 📚 Dataset Information
The dataset used for fine-tuning is available on Hugging Face:  

[![Hugging Face Dataset](https://img.shields.io/badge/HuggingFace-Dataset-yellow)](https://huggingface.co/datasets/Congliu/Chinese-DeepSeek-R1-Distill-data-110k)

## 🛠 Performance testing is currently in progress.
**Results and benchmarks will be shared soon!**

## 🔗 References
* [DeepSeek on Hugging Face](https://huggingface.co/deepseek-ai)
* [LoRA for Efficient Fine-Tuning](https://arxiv.org/abs/2106.09685)
* [Unsloth Library](https://github.com/unslothai/unsloth)

**🔥 Ready to fine-tune DeepSeek? Let’s go! 🚀**
