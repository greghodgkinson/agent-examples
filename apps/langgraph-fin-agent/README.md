# LangGraph Finance Agent

LangGraph Finance Agent is a financial assistant built using the LangGraph framework. It provides capabilities to query financial data about stocks, companies, and other financial metrics. Additionally, it can scrape web content to gather supplementary information.

## Features

- Retrieve current stock prices
- Fetch company profiles
- Obtain financial ratios and key metrics
- Retrieve market capitalization data
- Use stock screener for filtering stocks based on criteria
- Read and extract text content from web pages

## Installation

To install the LangGraph Finance Agent, follow these steps:

1. **Clone the repository:**

   ```bash
   git clone <repository-url>
   cd langgraph-fin-agent
   ```

2. **Install dependencies:**

   Ensure you have Python 3.11 installed. You can use [Poetry](https://python-poetry.org/) to manage dependencies:

   ```bash
   poetry install
   ```

   This will create a virtual environment and install all necessary dependencies.

   Note: I had to separately install beautiful soup.

   ```bash
   poetry add beautifulsoup4
   ```

## Configuration

1. **Set up environment variables:**

   Create a `.env` file in the root directory of the project containing your API keys and configurations. For example:

   ```plaintext
   FMP_API_KEY=<your_financial_modeling_prep_api_key>
   ```

## Usage

The LangGraph Finance Agent can be used in two modes: interactive mode and command-line query mode.

### Interactive Mode

To start an interactive session with the finance assistant, run:

```bash
poetry run python src/main.py
```

You can then ask questions about financial data and the assistant will provide responses based on available tools and web scraping capabilities.

### Command-Line Query Mode

To run a single query directly from the command line, use:

```bash
poetry run python src/main.py "your query here"
```

For example:

```bash
poetry run python src/main.py "What is the current stock price of AAPL?"
```

## Project Structure

- **`src/tools.py`**: Contains tools for making API requests and scraping web pages.
- **`src/graph.py`**: Defines the workflow and state graph for processing user queries.
- **`src/main.py`**: Entry point for running the application in interactive or single-query mode.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request if you would like to contribute.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact

For any inquiries, please contact Yi Zhang at yi@relari.ai.