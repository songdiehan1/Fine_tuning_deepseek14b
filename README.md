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
## 📚 Dataset Information
datasets/raw/zhihu_data.json → Zhihu Dataset (for QA-based conversational fine-tuning)

datasets/raw/xiaohongshu_data.json → Xiaohongshu Dataset (for social media text generation fine-tuning)

It is available on Hugging Face:  
[![Hugging Face Dataset](https://img.shields.io/badge/HuggingFace-Dataset-yellow)](https://huggingface.co/datasets/Congliu/Chinese-DeepSeek-R1-Distill-data-110k)







🔥 Ready to fine-tune DeepSeek? Let’s go! 🚀
