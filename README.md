# 🛍️ Multimodal AI Applications for E-Commerce Product Understanding

An end-to-end multimodal AI project developed as part of the **Gen AI Bootcamp Day 2**, demonstrating how state-of-the-art vision-language models can solve real-world e-commerce challenges such as intelligent product recommendation, catalog deduplication, and natural language product search.

---

## 📌 Project Overview

This notebook implements three practical multimodal AI applications by combining pretrained models and vector similarity search techniques.

The project showcases how **BLIP**, **CLIP**, **Vision Transformer (ViT)**, **Qwen-2.5**, **Faiss**, and **NetworkX** can work together to build scalable AI-powered e-commerce solutions without training custom deep learning models.

---

## ✨ Features

* 📷 Automatic product image caption generation
* 👔 AI-powered outfit recommendation
* 🔍 Cross-modal text-to-image product retrieval
* 🧹 Duplicate product detection and catalog cleaning
* ⚡ High-speed vector similarity search using Faiss
* 🖼️ Interactive visualization of retrieved products

---

# 🚀 Tasks Implemented

## Task 1: Smart Product Recommendation Engine

### Objective

Generate complementary fashion product recommendations from a single product image.

### Workflow

1. Generate product captions using **BLIP**
2. Pass captions to **Qwen-2.5** for complementary outfit suggestions
3. Encode suggestions using **CLIP Text Encoder**
4. Retrieve visually similar catalog images using **Faiss**
5. Display recommended products

### Technologies Used

* BLIP
* Qwen-2.5
* CLIP (ViT-B/32)
* Faiss
* PyTorch

---

## Task 2: Unique Product Catalog Creation

### Objective

Automatically identify duplicate and near-duplicate products to create a clean catalog.

### Workflow

1. Extract image embeddings using Vision Transformer (ViT)
2. Store embeddings in Faiss
3. Compute cosine similarity
4. Build similarity graph using NetworkX
5. Generate a duplicate-free product catalog

### Output

```
unique_product_catalog.csv
```

### Technologies Used

* Vision Transformer (ViT)
* Faiss
* NetworkX
* Pandas

---

## Task 3: Reverse Product Search

### Objective

Search products using natural language instead of keywords.

Example Queries

```
Blue striped shirt

Formal black shoes

White casual sneakers

Pink blouse
```

### Workflow

1. Encode text using CLIP Text Encoder
2. Encode images using CLIP Image Encoder
3. Perform nearest-neighbor search with Faiss
4. Retrieve top matching product images

### Technologies Used

* CLIP
* Faiss
* Transformers
* PyTorch

---

# 🛠️ Tech Stack

| Category               | Technologies    |
| ---------------------- | --------------- |
| Language               | Python          |
| Deep Learning          | PyTorch         |
| Vision-Language Models | BLIP, CLIP, ViT |
| Large Language Model   | Qwen-2.5        |
| Vector Database        | Faiss           |
| Graph Processing       | NetworkX        |
| Data Processing        | NumPy, Pandas   |
| Visualization          | Matplotlib      |

---

# 📂 Project Structure

```
.
├── AI&ML_task.ipynb
├── images/
├── unique_product_catalog.csv
├── README.md
└── requirements.txt
```

---

# ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/AlgorithmicNomad/AlgorithmicNomad.git
```

Move into the project directory

```bash
cd AlgorithmicNomad
```

Install the required packages

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

Open

```
AI&ML_task.ipynb
```

Run all cells sequentially.

---

# 📦 Required Libraries

```text
torch
torchvision
transformers
faiss-cpu
numpy
pandas
matplotlib
Pillow
networkx
scikit-learn
```

---

# 📊 Results

### ✅ Smart Recommendation Engine

* Generated descriptive captions from product images
* Produced AI-generated complementary outfit suggestions
* Retrieved visually relevant catalog products

### ✅ Product Catalog Deduplication

* Extracted image embeddings
* Grouped visually similar products
* Exported a clean catalog

### ✅ Reverse Product Search

* Supported natural language product search
* Retrieved visually relevant products without manual tags
* Demonstrated cross-modal retrieval using CLIP embeddings

---

# 💡 Applications

* E-commerce recommendation systems
* Fashion outfit suggestion
* Product catalog management
* Duplicate product detection
* Semantic image search
* AI-powered shopping assistants
* Inventory management

---

# 🔮 Future Improvements

* Fine-tune CLIP on domain-specific datasets
* Support multilingual product search
* Build a Streamlit web application
* Integrate with cloud vector databases
* Improve recommendation ranking using user behavior
* Add real-time product indexing

---

# 👨‍💻 Author

**Praful Rayamane**


GitHub: https://github.com/AlgorithmicNomad/AI-ML-Task

---

# 📜 License

This project is developed for educational and research purposes as part of the **Gen AI Bootcamp Day 2**.
