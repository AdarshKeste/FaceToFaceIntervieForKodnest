# F2F Technical Interview Platform

A web-based technical interview platform that uses AI to conduct and evaluate interviews.

## Local Development

1. Clone the repository:
```bash
git clone <your-repo-url>
cd <your-repo-name>
```

2. Create a `.env` file in the root directory and add your Gemini API key:
```
GEMINI_API_KEY=your_api_key_here
```

3. Serve the files using a local server. You can use Python's built-in server:
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

4. Open `http://localhost:8000` in your browser.

## Netlify Deployment

1. Push your code to GitHub.

2. Log in to Netlify and click "New site from Git".

3. Choose GitHub and select your repository.

4. In the deploy settings:
   - Build command: Leave empty
   - Publish directory: `.`

5. Click "Show advanced" and add the following environment variable:
   - Key: `GEMINI_API_KEY`
   - Value: Your Gemini API key

6. Click "Deploy site"

## Environment Variables

- `GEMINI_API_KEY`: Your Google Gemini API key (required)

## Features

- Real-time video interview
- AI-powered interview questions
- Speech-to-text for answers
- Performance evaluation
- Downloadable interview summary
- Video recording of the interview

## Security Note

Never commit your API keys to the repository. Always use environment variables for sensitive information. 