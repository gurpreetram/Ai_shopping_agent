
# AI Shopping Agent

An AI-powered shopping assistant built with Python, LangChain, Groq, Streamlit, and SQLite.

## Features

- Search products by keyword.
- Filter products by price and organic status.
- Retrieve product ratings and review counts.
- Analyze uploaded product images using a vision model.
- Place orders after user confirmation.
- Store product and order data in SQLite.

## Tech Stack

- Python
- LangChain Agents
- Groq API
- Streamlit
- SQLite
- uv for Python dependency management

## Project Structure

```text
shopping_agent/
├── app.py
├── shopping_agent.py
├── reviews_api.py
├── setup_db.py
└── resources/
```

## Setup

1. Install Python and uv.
2. Clone this repository.
3. Install dependencies:

   ```bash
   uv sync
   ```

4. Create a `.env` file in the project root:

   ```ini
   GROQ_API_KEY=your_groq_api_key_here
   ```

5. Start the application:

   ```bash
   uv run streamlit run shopping_agent/app.py
   ```

6. Open http://localhost:8501 in your browser.

## Security

- Never commit API keys or `.env` files.
- The local SQLite database is excluded from Git.
- Review database initialization behavior before running setup scripts.

## Status

Core text-based product search and image-based product search have been tested locally.
