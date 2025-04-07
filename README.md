# 📌 Resume Ranking App

## 🚀 Overview
The **Resume Ranking App** is a Python-based application that ranks resumes based on their relevance to a given job description. It leverages **TF-IDF** and **BERT embeddings** to compute similarity scores between resumes and job descriptions.

## 📂 Project Structure
```
📂 ResumeRankingApp
 ┣ 📂 data/                  # Sample CSV files for testing
 ┣ 📂 models/                # Pretrained models or serialized files (if applicable)
 ┣ 📜 requirements.txt       # Required dependencies
 ┣ 📜 README.md              # Detailed setup & usage instructions
 ┣ 📜 app.py                 # Main Gradio application file
 ┣ 📜 preprocess.py          # Preprocessing functions
 ┣ 📜 model.py               # Model loading and inference
 ┣ 📜 config.yaml            # Configuration file (optional)
 ┣ 📜 notebook.ipynb         # Jupyter Notebook with explanations & results
```

## 🛠️ Installation
To set up the environment, follow these steps:

### 1️⃣ Clone the repository
```bash
git clone https://github.com/yourusername/ResumeRankingApp.git
cd ResumeRankingApp
```

### 2️⃣ Create a virtual environment (optional but recommended)
```bash
python -m venv venv
source venv/bin/activate   # On Mac/Linux
venv\Scripts\activate     # On Windows
```

### 3️⃣ Install dependencies
```bash
pip install gradio
```

## ▶️ Running the Application
```bash
python app.py
```
The app will launch in your browser using **Gradio UI**.

## ▶️ Running The Video Explanation

https://drive.google.com/file/d/1yxtxQkCckXBR04zC-Uckf-8tvEPCFyMH/view?usp=sharing

## 📊 Model Explanation
The application uses:
- **TF-IDF Vectorization**: Converts text data into numerical vectors to compute cosine similarity.
- **BERT Sentence Embeddings**: Uses `all-mpnet-base-v2` from `sentence-transformers` to encode resumes and job descriptions.
- **Hybrid Score Calculation**: The final ranking is determined by combining TF-IDF and BERT scores.

## 🔄 Preprocessing Steps
- Text cleaning (lowercasing, removing special characters, stopwords, etc.).
- Combining relevant columns (e.g., skills, career objective, experience) into a single text field.
- Applying TF-IDF transformation.
- Generating BERT embeddings for more accurate similarity scoring.

## 📎 Sample CSV Format
| skills | career_objective | degree_names | major_field_of_studies | positions | responsibilities |
|--------|-----------------|--------------|------------------------|-----------|------------------|
| Python, ML | Data Scientist Role | B.Tech | Computer Science | Developer | AI Model Training |

## 📌 Contribution
Feel free to fork this repository and submit a pull request if you'd like to contribute!

## 📞 Contact
For any issues, reach out via GitHub Issues.

