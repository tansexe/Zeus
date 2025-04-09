# ZEUS: A Weather Dashboard

A modern, responsive weather application built with React that provides real-time weather information for any city worldwide.

<img width="960" alt="image" src="https://ik.imagekit.io/Eattendancehostel23/Screenshot%202025-04-09%20223001.png?updatedAt=1744218074815">

## Features

- **City Search**: Look up current weather for any city around the world
- **Weather Details**: View comprehensive weather information including:
  - Current temperature (°C)
  - Weather conditions with icons
  - Feels like temperature
  - Humidity levels
  - Wind speed
  - Atmospheric pressure
- **Search History**: Automatically saves and displays your five most recent searches
- **Refresh Function**: Update current weather data with a single click
- **Responsive Design**: Fully optimized for both desktop and mobile devices
- **Error Handling**: User-friendly error messages for invalid cities or API issues
- **Loading States**: Visual feedback during data fetching

## Tech Stack

- **Frontend Framework**: React.js (Vite)
- **State Management**: React Hooks
- **API Integration**: OpenWeatherMap API
- **Styling**: CSS with custom variables for theming
- **HTTP Client**: Native fetch API
- **Storage**: localStorage for search history persistence
- **Deployment**: Vercel

## Setup Instructions

### Prerequisites

- Node.js (v14.0.0 or later)
- npm or yarn
- OpenWeatherMap API key (see API Integration section)

### Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/weather-dashboard.git
cd frontend
```

2. Install dependencies:

```bash
npm install
# or
yarn
```

3. Create a `.env` file in the project root and add your OpenWeatherMap API key:

```
VITE_OPENWEATHER_API_KEY=your_api_key_here
```

4. Start the development server:

```bash
npm run dev
# or
yarn dev
```

5. Open your browser and navigate to `http://localhost:5173`

## API Integration

This project uses the OpenWeatherMap API to fetch weather data.

### API Key

- Sign up for a free API key at [OpenWeatherMap](https://openweathermap.org/api)
- Free tier includes 1,000 API calls per day
  
### Endpoints Used

- Current Weather: `https://api.openweathermap.org/data/2.5/weather`
  - Parameters:
    - `q`: City name
    - `appid`: Your API key
    - `units`: Metric (for Celsius)

### Rate Limits

- Free tier: 60 calls per minute
- If you exceed the limits, the API will return a 429 error

## Project Structure

```
src/
├── components/
│   ├── SearchForm.jsx       # City search input and button
│   ├── SearchHistory.jsx    # Recent searches display
│   ├── WeatherDisplay.jsx   # Weather information card
│   ├── ErrorMessage.jsx     # Error notification component
│   └── LoadingSpinner.jsx   # Loading indicator
├── services/
│   └── weatherService.js    # API integration functions
├── App.jsx                  # Main application component
├── App.css                  # Global styles
└── main.jsx                 # Entry point
```

## Usage

1. Enter a city name in the search box
2. Press Enter or click the Search button
3. View detailed weather information
4. Click on any city in your search history to quickly look it up again
5. Use the refresh button (↻) to update the weather data

## Deployment

The application is deployed on Vercel and can be accessed at [Live URL](https://weather-app-one-brown-76.vercel.app/).

## Final Video
<video src="[path/to/video.mp4](https://ik.imagekit.io/Eattendancehostel23/Screen%20Recording%202025-04-09%20222727(1).mp4?updatedAt=1744219941296)" width="320" height="240" controls></video>



## Future Enhancements

- Dark/Light theme toggle
- 5-day weather forecast
- Weather maps integration
- Temperature unit conversion (°C/°F)
- Geolocation-based weather detection

## Credits

- Weather data provided by [OpenWeatherMap](https://openweathermap.org/)
- Weather icons from [OpenWeatherMap](https://openweathermap.org/weather-conditions)
- Created as part of the Frontend Developer Assessment

---
