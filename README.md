
# AI Driving Assistant 🚗🧠

A real-time car safety chatbot that leverages **Google Gemini AI**, **FAISS vector search**, and a curated knowledge base to provide drivers with instant, expert guidance on drowsiness prevention, emergency handling, and safe driving practices.

---

## 🔧 Features

- **Contextual Car Safety Chatbot**  
  Ask any driving safety question and get structured, actionable advice.

- **FAISS-Powered Knowledge Retrieval**  
  Fast, relevant retrieval from a curated car safety knowledge base.

- **Google Gemini 2.0 Integration**  
  Generates clear, expert-level responses using the latest generative AI.

- **Asynchronous Processing**  
  Handles multiple requests efficiently using threading and queues.

- **REST API with Flask**  
  Simple `/chat` endpoint for integration with apps or other services.

- **CORS Enabled**  
  Ready for cross-origin requests from web/mobile clients.

---

## 🚀 Quick Start

```bash
git clone https://github.com/yourusername/ai-driving-assistant.git
cd ai-driving-assistant
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate
pip install -r requirements.txt
echo "GOOGLE_API_KEY=your_gemini_api_key_here" > key.env
python app.py
```

---

## 🧪 API Usage

### `/chat` Endpoint

- **Method:** `POST`  
- **Content-Type:** `application/json`  
- **Body Example:**
```json
{
  "query": "How can I prevent drowsy driving?"
}
```

- **Sample Response:**
```json
{
  "response": "1. Take regular breaks every 2 hours...\n2. Stay hydrated...\n3. Avoid heavy meals before driving..."
}
```

---

## 📚 Knowledge Base Topics

- Drowsiness Prevention  
- Fatigue Signs  
- Defensive Driving  
- Weather Conditions  
- Emergency Handling  
- Vehicle Maintenance  
- Night Driving  
- Distraction Prevention  
- Crash Prevention  
- First Aid Kit Essentials

---

## ⚙️ How It Works

1. User submits a driving safety question via the `/chat` endpoint.  
2. FAISS retrieves the most relevant safety knowledge snippets.  
3. Google Gemini 2.0 generates a detailed, structured response using the context.  
4. Response is returned in clear, actionable steps.

---

## 📦 Requirements

- Python 3.9+  
- Flask  
- Flask-CORS  
- FAISS (faiss-cpu)  
- numpy  
- python-dotenv  
- google-generativeai  

Install all dependencies with:

```bash
pip install -r requirements.txt
```

---

## 🤝 Contributing

Pull requests, issues, and suggestions are welcome!  
Please open an issue to discuss your ideas or report bugs.

## 🙏 Acknowledgements

- [Google Gemini API](https://ai.google.dev/)
- [FAISS by Facebook AI Research](https://github.com/facebookresearch/faiss)
- [Flask Web Framework](https://flask.palletsprojects.com/)

> Drive safe, drive smart! 🚦


