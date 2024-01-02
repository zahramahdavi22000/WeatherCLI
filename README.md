# Weather CLI
This repository contains a simple weather cli application that fetches temperatures for various cities using a API.

## Preview
```
------------------------
        Weather
------------------------
> enter your city: tehran
tehran temp is 20°C
```

## Description
This Python project utilizes Flask for creating a local weather API and fetching temperature data from a predefined set of cities. It consists of two main components:

- **Client Script (`cli.py`):**
  - Fetches temperature data for a specified city using the API endpoints.
  - Allows users to input their city to get the current temperature.

- **Server (`api.py`):**
  - Provides API endpoints to get temperature data for cities, add new city temperatures, and retrieve all stored temperatures.
  - Utilizes Flask and a JSON file (`temps.json`) to store and manage temperature data.

## Requirements
- Python 3.x
- Flask (`pip install flask`)
- Requests (`pip install requests`)


### Server
1. Run the `api.py` script.
2. The server will start locally on port 8000.
3. Access the following endpoints:
   - `/`: Home route indicating that the Weather API is running.
   - `/get_temp?city=<city_name>`: Get the temperature for a specific city.
   - `/get_temps`: Get temperatures for all cities.
   - `/add_temp?city=<city_name>&temp=<temperature>`: Add or update the temperature for a city.

### Client
1. Run the `cli.py` script.
2. Enter the name of the city when prompted.
3. View the current temperature for the entered city.

## Note
- The server uses a JSON file (`temps.json`) to store temperature data persistently.

Feel free to contribute, report issues, or suggest improvements!