# 👗 StyleAI - AI-Powered Fashion Styling Advisor

StyleAI is a professional web application that leverages **Groq's LLaMA 3.3 70B** AI model to provide comprehensive personal styling recommendations. The application analyzes user photos to detect skin tone and generates personalized fashion advice, including outfit suggestions, color palettes, and curated shopping links.

---

## ✨ Features

### 🎯 Skin Tone Analysis
- Automatically detects skin tone from uploaded photos.
- Categories:
  - Fair
  - Medium
  - Olive
  - Deep

### 🤖 AI Fashion Consultant
- Powered by **LLaMA 3.3 70B** through the Groq API.
- Generates personalized styling recommendations.

### 👥 Gender-Specific Recommendations
Tailored fashion suggestions for:
- Male
- Female
- Non-Binary

### 🛍️ Smart Shopping Assistance
- Provides vendor-agnostic Google Shopping search links.
- Helps users find recommended clothing items across multiple retailers.

### ⚡ Fast & Professional
- Built using Flask and modern web technologies.
- Responsive and user-friendly interface.

---

## 🖼️ Application Workflow

1. **Upload Photo**
   - Upload a clear facial image (JPG or PNG).

2. **Select Gender**
   - Choose Male, Female, or Non-Binary.

3. **Skin Tone Detection**
   - Computer vision analyzes the image.

4. **AI Styling Recommendations**
   - LLaMA 3.3 70B generates personalized outfit suggestions.

5. **Shopping Suggestions**
   - Receive Google Shopping search links for recommended items.

---

## 🛠️ Tech Stack

| Component | Technology |
|------------|------------|
| Backend | Flask (Python) |
| Frontend | HTML5, CSS3, Bootstrap 5, JavaScript |
| AI Model | Groq LLaMA 3.3 70B |
| Image Processing | OpenCV, PIL, NumPy |
| Environment Management | Python-dotenv |

---

## 📋 Prerequisites

Before running the project, ensure you have:

- Python 3.8 or higher
- Groq API Key (Free tier available)
- pip package manager

---

## 🚀 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/Generative_AI_Powered_Fashion_Recommendation.git
cd Generative_AI_Powered_Fashion_Recommendation
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Configure Groq API Key

#### Option A: Environment Variable (Recommended)

Create a `.env` file in the project root:

```env
GROQ_API_KEY=your_groq_api_key_here
```

Get your API key from the Groq Console.

#### Option B: Enter API Key in the Web Interface

Leave the `.env` file empty and paste the API key directly into the application when it loads.

---

## ▶️ Running the Application

Start the Flask server:

```bash
python app_flask.py
```

The application will be available at:

```text
http://127.0.0.1:5000
```

Open the URL in your browser to start using StyleAI.

---

## 📁 Project Structure

```text
Generative_AI_Powered_Fashion_Recommendation/
│
├── app_flask.py              # Flask application entry point
├── utils.py                  # Image processing & skin tone detection
├── groq_client.py            # Groq API integration
├── requirements.txt          # Python dependencies
├── .env                      # Environment variables
│
├── templates/
│   └── index.html            # Main web interface
│
└── static/
    ├── style.css             # Application styling
    └── script.js             # Frontend interactions
```

---

## 🔍 How Skin Tone Detection Works

The system uses computer vision techniques to:

1. Detect the user's face.
2. Extract facial skin regions.
3. Analyze dominant skin color.
4. Classify skin tone into predefined categories.
5. Use the detected tone to personalize fashion recommendations.

---

## 🧠 AI Recommendation Engine

StyleAI utilizes **Groq's LLaMA 3.3 70B** model to generate:

- Outfit combinations
- Seasonal fashion advice
- Color coordination tips
- Accessory suggestions
- Occasion-specific styling
- Shopping recommendations

---

## 📸 Best Photo Guidelines

For accurate analysis:

✅ Use a clear front-facing photo

✅ Ensure good lighting

✅ Avoid heavy filters

✅ Remove sunglasses

✅ Keep the face unobstructed

❌ Avoid blurry images

❌ Avoid dark lighting conditions

---

## 🛒 Shopping Recommendations

The application provides:

- Outfit suggestions
- Color-matched clothing ideas
- Google Shopping search links
- Vendor-independent recommendations

Users can compare products from multiple online retailers.

---

## ❗ Troubleshooting

### "No Face Detected"

Possible solutions:

- Upload a clearer image.
- Ensure the face is visible.
- Use better lighting.
- Remove hats, masks, or sunglasses.

---

### "API Key Is Missing"

Make sure:

```env
GROQ_API_KEY=your_api_key_here
```

exists in your `.env` file.

Alternatively, enter the API key through the application interface.

---

### Port Already in Use

Modify the port in `app_flask.py`:

```python
app.run(debug=True, host="127.0.0.1", port=5001)
```

Then access:

```text
http://127.0.0.1:5001
```

---

## 📦 Key Dependencies

```text
Flask
OpenCV
NumPy
Pillow
python-dotenv
Groq SDK
```

Install all dependencies using:

```bash
pip install -r requirements.txt
```

---

## 🔒 Privacy

- Images are processed only for styling analysis.
- No permanent image storage is required.
- API keys remain under user control.

---

## 🌟 Future Enhancements

- Virtual outfit try-on
- Seasonal trend analysis
- Celebrity-inspired looks
- Fashion mood boards
- Wardrobe management
- Multi-image analysis
- Personalized style history

---

## 📄 License

This project is open-source and available under the MIT License.

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch

```bash
git checkout -b feature-name
```

3. Commit your changes

```bash
git commit -m "Add feature"
```

4. Push to GitHub

```bash
git push origin feature-name
```

5. Open a Pull Request

---

## 📞 Support

If you encounter any issues:

- Verify Python 3.8+ installation
- Confirm Groq API configuration
- Reinstall dependencies
- Review Flask console logs

For additional documentation:

- Groq Documentation: https://groq.com/docs

---

### ⭐ If you find this project useful, consider giving it a star on GitHub!
