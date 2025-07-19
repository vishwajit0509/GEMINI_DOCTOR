# Nutrition Advisor App 🥗

A smart nutrition analysis tool that uses Google's Gemini AI to analyze food images and provide detailed nutritional insights, calorie counts, and health recommendations.

## Features ✨

- **Image-based Food Analysis**: Upload photos of meals to get instant nutritional analysis
- **Calorie Calculation**: Accurate calorie estimation for individual food items and total meal
- **Nutritional Breakdown**: Detailed analysis of carbohydrates, fats, proteins, fiber, and sugar content
- **Health Assessment**: AI-powered recommendations on whether the meal is healthy
- **Interactive Web Interface**: User-friendly Streamlit-based web application
- **Real-time Processing**: Instant results using Google Gemini 1.5 Flash model

## Tech Stack 🛠️

- **Frontend**: Streamlit
- **AI Model**: Google Gemini 1.5 Flash API
- **Image Processing**: PIL (Python Imaging Library)
- **Environment Management**: python-dotenv
- **Language**: Python 3.x

## Installation 📦

### Prerequisites
- Python 3.7 or higher
- Google API key for Gemini AI
- pip package manager

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd nutrition-advisor
   ```

2. **Install required packages**
   ```bash
   pip install streamlit -r requirements.txt
   ```

3. **Set up environment variables**
   - Create a `.env` file in the project root
   - Add your Google API key:
     ```
     GOOGLE_API_KEY=your_google_api_key_here
     ```

4. **Get Google API Key**
   - Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
   - Generate a new API key
   - Copy the key to your `.env` file

## Usage 🚀

1. **Start the application**
   ```bash
   streamlit run app.py
   ```

2. **Using the app**
   - Open your browser and navigate to `http://localhost:8501`
   - Enter an optional text prompt for specific analysis requests
   - Upload an image of your meal (supported formats: JPG, JPEG, PNG)
   - Click "Tell me the total calories" to get the analysis

3. **Understanding the results**
   - Individual food items with calorie counts
   - Total meal calories
   - Health assessment (healthy/unhealthy)
   - Nutritional breakdown percentages
   - Dietary recommendations

## Project Structure 📁

```
nutrition-advisor/
│
├── app.py                 # Main Streamlit application
├── .env                   # Environment variables (create this)
├── .env.example          # Example environment file
├── requirements.txt      # Python dependencies
└── README.md            # Project documentation
```

## Sample Output 📊

The app provides analysis in the following format:

```
1. Grilled Chicken Breast - 185 calories
2. Brown Rice (1 cup) - 216 calories
3. Mixed Vegetables - 80 calories
----
Total Calories: 481

Health Assessment: This meal is healthy and well-balanced.

Nutritional Breakdown:
- Carbohydrates: 45%
- Proteins: 35% 
- Fats: 15%
- Fiber: 3%
- Sugar: 2%
```

## API Usage 🔧

The app uses Google's Gemini 1.5 Flash model for:
- Food item identification
- Calorie estimation
- Nutritional analysis
- Health recommendations

## Supported Image Formats 📷

- JPG/JPEG
- PNG

## Error Handling 🛡️

- File upload validation
- API error handling
- Image format verification
- Environment variable checks



## Future Enhancements 🔮

- [ ] Support for multiple images
- [ ] Meal history tracking
- [ ] Export analysis reports
- [ ] Custom dietary goals
- [ ] Barcode scanning integration
- [ ] Recipe suggestions
- [ ] Portion size recommendations



### Error Messages

- `FileNotFoundError: No file uploaded` - Upload an image before analysis
- `API Key not found` - Check your `.env` file configuration

## License 📄

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments 🙏

- Google Gemini AI for providing the powerful vision capabilities
- Streamlit for the excellent web framework
- PIL for image processing utilities



---

**Note**: This application is for informational purposes only and should not replace professional nutritional advice. Always consult with healthcare professionals for dietary decisions.
