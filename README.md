# Weather API Application

A simple desktop application to check weather for any city in the world. Built with Python using PyQt5 GUI framework and integrated with OpenWeatherMap API to fetch real-time weather data.

## Features

- Search weather by city name
- Display temperature in both Celsius and Fahrenheit
- Show weather emoji and description
- Handle basic errors (city not found, connection issues, etc.)

## Requirements

- Python 3.7+
- PyQt5
- requests
- Internet connection

## Installation

Install required dependencies:
```bash
pip install PyQt5 requests
```

Run the application:
```bash
python main.py
```

## Usage

1. Run the app: `python main.py`
2. Enter a city name in the input field
3. Click the "Get Weather" button
4. View the temperature, emoji, and weather description

## Code Structure

**API Used**: OpenWeatherMap (https://api.openweathermap.org/data/2.5/weather)

**Main Functions**:
- `init_ui()`: Initialize UI components
- `get_weather()`: Fetch weather data from API
- `display_weather()`: Update UI with results
- `get_weather_emoji()`: Convert weather code to emoji

## Notes

The API key is currently hardcoded in the code. For production applications, use environment variables instead.

## What I Learned

Through this project, I learned:
- How to build GUI applications with PyQt5
- Integration with external APIs using HTTP requests
- Error handling and data validation
- Parsing JSON responses from APIs

---

**Created**: Python 12 Hours Project  
**Last Updated**: January 2026  
**Status**: ✓ Basic implementation complete
