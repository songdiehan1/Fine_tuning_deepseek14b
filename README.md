# 🚀 DeepSeek-14B Fine-Tuning Project
This project aims to fine-tune DeepSeek-R1-Distill-Qwen-14B using Zhihu and Xiaohongshu datasets separately. The fine-tuning is conducted using the LoRA method with the Unsloth framework, optimized for Colab + A100 with BF16 support. The repository includes scripts for model training, evaluation, and inference.

## 📁 Project Structure

## 🚀 Features
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
│── models/                          # Fine-tuned models
│   ├── zhihu_lora_adapter/          
│   ├── xhs_lora_adapter/    
│── training/                        
│   ├── train_zhihu.py               
│   ├── train_xhs.py         
│── inference/                       
│   ├── inference_zhihu.py           
│   ├── inference_xhs.py
│── scripts/                       
│   ├──zhihu_colab_demo.ipynb            
│   ├──xhs_colab_demo.ipynb
│── wandb/                       
│   ├──zhihu_train_loss.png           
│   ├──xhs_train_loss.png                   
│── requirements.txt                 
│── README.md                        
```








🔥 Ready to fine-tune DeepSeek? Let’s go! 🚀
