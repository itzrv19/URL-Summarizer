# Smart URL Summarizer (Flask API)
A lightweight API that shortens URLs, tracks clicks, and generates AI summaries of webpage content.

## Features
- Shorten long URLs with unique hashes
- Redirect to original pages
- AI-based webpage summarization using Hugging Face (T5)
- Track click counts per URL

## Tech Stack
- Python
- Flask
- Hugging Face Transformers (T5-small)
- BeautifulSoup4
- JSON-based storage
Screenshots
<img width="1919" height="1020" alt="Screenshot 2026-04-22 121213" src="https://github.com/user-attachments/assets/d55e9ed2-00ff-49b3-9c4f-0af51460f805" />
<img width="1919" height="1017" alt="Screenshot 2026-04-22 122627" src="https://github.com/user-attachments/assets/0075a68c-2448-44a2-b330-db284e56e62f" />
<img width="1916" height="1021" alt="Screenshot 2026-04-22 121715" src="https://github.com/user-attachments/assets/3c730a78-47de-43fd-b427-cc61998fc664" />

## API Routes
| Method | Endpoint | Description |
|--------|-----------|-------------|
| POST | `/shorten` | Shorten URL and summarize webpage |
| GET | `/<short_id>` | Redirect to original page |
| GET | `/stats/<short_id>` | View analytics & summary |

## Run Locally
```bash
git clone https://github.com/itzrv19/URL-Summarizer
cd url-summarizer
pip install -r requirements.txt
python app.py


