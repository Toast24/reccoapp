# ReccoApp 🎬

ReccoApp is a lightweight movie recommendation application that suggests **5 movies similar** to any movie you enter. It uses a dataset of 5000 films and a cosine-similarity machine learning model to generate fast and relevant recommendations.

---

## 🚀 Features

- 🎯 Enter a movie → get **5 similar recommended movies**
- ⚙️ Powered by **cosine similarity**
- 🧠 Uses precomputed **pickle-serialized model files**
- 🎨 Clean and simple **Streamlit** UI
- 📁 Fully local — no external APIs required

---

## 🧠 How It Works

1. Loads metadata from the TMDB 5000 movie dataset  
2. Converts each movie into a feature vector  
3. Uses **cosine similarity** to compare movies  
4. Returns the **top 5 most similar** movies  

---

## 🛠 Tech Stack

- Python  
- Pandas / NumPy  
- scikit-learn  
- Streamlit  
- Pickle  

---

## 📦 Getting Started

### ✔ Prerequisites

- Python **3.7+**
- `pip` or a virtual environment

---

## 🔧 Installation

Clone the repository:

```bash
git clone https://github.com/Toast24/reccoapp.git
cd reccoapp
```

(Optional) Create a virtual environment:

```bash
python3 -m venv venv
source venv/bin/activate       # Windows: venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Ensure the following files exist:

- `movies.pkl`
- `movie_dict.pkl`
- `similarity.pkl`

---

## ▶ Running the App

Start the Streamlit application:

```bash
streamlit run app.py
```

Then open the provided local URL (usually `http://localhost:8501`).

---

## 🎮 Usage

1. Open the Streamlit page  
2. Enter the name of any movie  
3. Click **Recommend**  
4. View a list of 5 similar movies  

---

## 📁 Project Structure

```
reccoapp/
├── app.py               # Streamlit app UI
├── main.py              # Core movie recommendation logic
├── movies.pkl           # Movie dataset
├── movie_dict.pkl       # Dictionary of movie metadata
├── similarity.pkl       # Precomputed similarity matrix
├── requirements.txt     # Python dependencies
├── setup.sh             # Optional setup script
└── README.md            # Documentation
```

---

## 🐞 Known Issues / Limitations

- Only supports movies included in the TMDB-5000 dataset  
- Model is static — no dynamic training  
- Basic UI with limited filtering options  

---

## 🛣 Future Improvements

- Add movie posters & metadata to the UI  
- Improve the recommendation algorithm using NLP embeddings  
- Add category-based recommendations  
- Dockerize and deploy the app  
- Allow users to rate recommendations  

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository  
2. Create a feature branch  
3. Commit your changes  
4. Open a pull request  

---

## 📜 License

This project is licensed under the **MIT License**.  
(Feel free to replace with another license.)

---

## 📬 Contact

**Author:** Toast24  
For issues or suggestions, please open a GitHub issue.
