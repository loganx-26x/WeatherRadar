# Weather Analyzer and Trends Application

## Overview

This Django-based web application serves as a comprehensive weather data aggregator, analyzer, and trend visualizer. It fetches real-time weather data from public APIs, stores it in a database, and provides users with insightful analysis and visualizations of weather trends over time.

## Features

- Real-time weather data fetching from public APIs
- Weather trend analysis and visualization
- User-friendly interface for location-based weather queries
- Responsive design for both desktop and mobile use

## Prerequisites

- Python 3.8+
- Django 3.2+
- Other required packages (see `requirements.txt`)

## Setup

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/weather-analyzer-app.git
cd weather-analyzer-app
```

### 2. Set Up a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Set Up Environment Variables

Create a `.env` file in the root directory of the project and add the following variables:

```
SECRET_KEY=your_django_secret_key
DEBUG=True
OPENWEATHER_KEY=your_weather_api_key
```

Replace the placeholder values with your actual data:
- `your_django_secret_key`: A secure random string for Django's SECRET_KEY
- `your_weather_api_key`: Your API key for the weather data service
- `your_database_url`: URL for your database (e.g., `postgres://user:password@localhost/dbname`)

### 5. Database Setup

```bash
python manage.py migrate
```

### 6. Run the Development Server

```bash
python manage.py runserver
```

The application should now be accessible at `http://localhost:8000`.

## Usage

1. Navigate to the home page.
2. Enter a location in the search bar.
3. View current weather data and trend analysis for the specified location.

## API Reference

Our application uses the [OpenWeatherMap API](https://openweathermap.org/api) for fetching weather data. Refer to their documentation for more details on the data structure and available endpoints.

## Acknowledgments

- OpenWeatherMap for providing the weather data API
- Django community for the robust web framework