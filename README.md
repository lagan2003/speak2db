# 🧠 Speak2DB – Voice to SQL using Gemini + Streamlit

🎯 **Speak2DB** lets you ask questions in plain English or voice and get real-time SQL results from an SQLite database — powered by **Google Gemini API** and displayed through a **Streamlit interface**.

---

## ⚙️ Tech Stack

- **Language:** Python  
- **Database:** SQLite  
- **AI Model:** Google Gemini  
- **Frontend:** Streamlit  
- **Voice Input:** `streamlit-webrtc`  
- **Text-to-Speech:** `gTTS`  

---

## 🚀 Features

✅ Ask questions by voice or text  
✅ Gemini generates SQL queries based on your schema  
✅ Results shown in table & chart form  
✅ Summarized output spoken aloud  
✅ Works on cloud with no local dependencies

---

## 🧾 Dataset Used

- Tables: `CustomerTable`, `SalesTable`, `TransactionLog`
- Loaded into `sales_database.db`

---

## 🔧 Setup

```bash
git clone https://github.com/lagan2003/speak2db.git
cd speak2db

# Add your Gemini API key
echo GOOGLE_API_KEY="your-key" > .env

# Create & activate virtual environment
python -m venv venv
venv\Scripts\activate  # or source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# (Optional) Initialize DB
python sql.py

# Run app
streamlit run app.py

