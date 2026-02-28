# AI-Agents Project

This repository contains multiple AI-powered agents designed to solve real-world problems using Python and Jupyter Notebooks. Each agent is organized in its own directory with a dedicated notebook and supporting files. The project demonstrates modular AI agent design, secure API usage, and practical applications of NLP and data retrieval.

## Project Structure

- `restaurent-query-agent/`
    - Implements a chatbot for restaurant FAQs using PDF document retrieval and NLP.
    - Main file: `bucket.fud.ipynb`
    - Expected supporting file: `The_Bucket.fud_FAQ.pdf` (not included)
    - [See detailed README in the directory.](restaurent-query-agent/README.md)

- `weather-agent/`
    - Implements a conversational weather information agent using a public weather API.
    - Main file: `weather-agent.ipynb`
    - [See detailed README in the directory.](weather-agent/README.md)

## Tech Stack

- **Python 3.x**
- **Jupyter Notebook**
- **Key Libraries:**
    - `requests` — For HTTP requests to APIs
    - `python-dotenv` — For secure environment variable management
    - `os` — For environment variable access
    - `nltk` — For natural language processing (restaurant agent)
    - `scikit-learn` — For TF-IDF vectorization and similarity (restaurant agent)
    - `PyPDF2` — For PDF text extraction (restaurant agent)

## Security & Best Practices

- API keys are loaded from environment variables using `.env` files and never hardcoded.
- `.env` files should be included in `.gitignore` to prevent accidental exposure of sensitive information.
- Each agent is modular and can be extended or integrated with other services.

## Getting Started

1. Clone the repository:
    ```sh
    git clone https://github.com/Dr-Stitch/AI-Agents.git
    ```
2. Follow the setup instructions in each agent's directory README.
3. Install required Python packages as listed in the notebooks or READMEs.
4. Place any required data files (e.g., PDFs, .env) in the appropriate directories.
5. Open and run the notebooks in Jupyter or VS Code.

## Agents Overview

### Restaurant Query Agent

- Answers customer questions by searching a PDF FAQ document.
- Uses NLP and vector similarity to find the most relevant answer.
- Modular design for easy extension (e.g., memory, LLM integration).

### Weather Agent

- Retrieves current weather information for any city using a public API.
- Stores and recalls previous queries for context.
- Demonstrates secure API key handling and conversational response generation.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for improvements or new agents.

## License

This project is licensed under the MIT License.

## Contact

For questions or suggestions, please contact the project maintainer or open an issue in this repository.
