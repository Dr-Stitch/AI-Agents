# Weather Agent

This directory contains the implementation of a weather information retrieval agent using Python. The main file, `weather-agent.ipynb`, demonstrates how to build a simple conversational agent that fetches and presents current weather data for a given city.

## File Overview

### `weather-agent.ipynb`

- **Type:** Jupyter Notebook
- **Purpose:** Provides a step-by-step guide and code for building a weather chatbot agent.
- **Key Features:**
    - Loads the OpenWeather API key securely from environment variables (using a `.env` file and `python-dotenv`).
    - Defines a `WeatherRetrievalAgent` class to fetch weather data from the WeatherAPI service.
    - Implements a `MemoryAgent` class to store and recall previous weather queries.
    - Includes a `ResponseAgent` class to generate user-friendly responses.
    - Demonstrates a simple workflow: user inputs a city, the agent fetches weather data, stores the query, and prints a formatted response.

## Setup Instructions

1. **Install Required Packages:**
    ```python
    !pip install requests python-dotenv
    ```
2. **API Key Setup:**
    - Create a `.env` file in this directory with the following content:
        ```
        OPENWEATHER_API_KEY=your_api_key_here
        ```
    - Replace `your_api_key_here` with your actual OpenWeather API key.

3. **Run the Notebook:**
    - Open `weather-agent.ipynb` in Jupyter or VS Code.
    - Execute the cells in order to interact with the weather agent.

## How It Works

- The user is prompted to enter a city name.
- The `WeatherRetrievalAgent` fetches current weather data for the city.
- The `MemoryAgent` stores each query and its result.
- The `ResponseAgent` generates a human-readable summary of the weather.
- The notebook prints the response and the memory of all previous queries.

## Security Note

- The API key is loaded from an environment variable for security. Do not hardcode your API key in the notebook.
- The `.env` file should be included in `.gitignore` to prevent accidental commits of sensitive information.

## Customization

- You can extend the agent to support more weather features, integrate with other APIs, or improve the conversation flow.

## Contact

For questions or suggestions, please contact the project maintainer or open an issue in your repository.
