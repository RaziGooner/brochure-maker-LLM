# Brochure Maker with LLM

This project uses a large language model (LLM) to extract all the hyperlinks from a given webpage and generate a professionally worded brochure or summary using those links. The idea is to automate brochure generation based on website content.

## 📌 Features

- Automatically scrapes all hyperlinks from a provided webpage URL.
- Uses BeautifulSoup for HTML parsing.
- Formats the extracted links and their surrounding context into a markdown-based summary.
- Uses OpenAI's GPT model to generate a coherent, human-readable brochure-style content.

## 🧠 How It Works

1. **Input a URL** of a webpage.
2. The script:
   - Sends a GET request to the webpage.
   - Parses the page using `BeautifulSoup`.
   - Extracts all hyperlinks (`<a href="...">` tags).
3. The extracted links and surrounding text are passed to a language model (via OpenAI's API or similar).
4. The model returns a brochure-style summary or description that highlights key parts of the site.
5. The result is displayed or saved in markdown/HTML format.

## 📦 Requirements

- Python 3.8+
- `requests`
- `beautifulsoup4`
- `openai`
- `python-dotenv` (optional, if using API keys from a `.env` file)

Install all required packages with:

```bash
pip install -r requirements.txt
