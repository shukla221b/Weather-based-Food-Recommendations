---

## 🌦️ Weather-Based Meal & Workout Recommendation App

This Python project recommends healthy meals and personalized workouts based on the weather conditions of your city. It leverages weather forecasts, AI suggestions, APIs, and web scraping to give dynamic recommendations for food and fitness.

---

### 🚀 Features

- 🌤️ **Weather Forecasting**: Fetches 3-day weather data for your location using OpenWeather API.
- 🥗 **Meal Recommendations**:
  - Fetches healthy recipes via the Spoonacular API.
  - Scrapes curated recipes from food blogs as backups.
- 🏋️ **Workout Suggestions**:
  - Scrapes Wikipedia to build an exercise database.
  - Recommends workouts tailored to the weather (indoor, outdoor, strength, etc.).
- 🤖 **AI Integration**: Uses Cloudflare AI to generate custom meal and fitness suggestions.
- 🧠 **Fallback Logic**: Uses cached data or defaults if API/web scraping fails.

---

### 🧰 Technologies Used

- Python 3.x
- APIs: OpenWeather, Spoonacular, Cloudflare AI
- Libraries: `requests`, `pandas`, `BeautifulSoup`, `time`, `random`, `os`

---

### 🛠️ Setup Instructions

1. **Clone the repository**  
   ```bash
   git clone https://github.com/shukla221b/weather-meal-workout.git
   cd weather-meal-workout
   ```

2. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up environment variables**  
   Create a `.env` file or export these:
   ```bash
   export CLOUDFLARE_API_KEY=your_cloudflare_key
   export OPENWEATHER_API_KEY=your_openweather_key
   export SPOONACULAR_API_KEY=your_spoonacular_key
   ```

4. **Run the notebook**
   
   WBFR.ipynb
   


---

### 📸 Sample Output

```plaintext
📅 Date: 2025-03-04
⛅ Weather: clear sky | Temperature: 25.9°C

🍽 API RECOMMENDED RECIPE:
   Pork Schnitzel And Apple Salad (http://www.foodista.com/...)

💪 WORKOUT RECOMMENDATION:
   Outdoor activity: Focus on lower body exercises
   1. Leg press (targets: Gluteus, Quads)
   2. Lunges (targets: Hamstrings, Gluteus) ...
```

---

### 📁 Project Structure

```
├── main.py
├── weight_training_exercises.csv  # generated if scraping succeeds
├── README.md
├── requirements.txt
└── .env (your secret keys)
```

---

### 📌 Notes

- If scraping fails, fallback CSV or default workouts are used.
- Add error handling/logging as needed for production readiness.

---

### 🙌 Acknowledgments

- [OpenWeather](https://openweathermap.org/)
- [Spoonacular](https://spoonacular.com/food-api)
- [Pinch of Yum](https://pinchofyum.com/)
- [Cloudflare AI](https://developers.cloudflare.com/ai/)
- [Wikipedia](https://en.wikipedia.org/wiki/List_of_weight_training_exercises)

---

Let me know if you want help customizing the project name, adding badges, or generating a `requirements.txt`.
