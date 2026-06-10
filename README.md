# Bitcoin AI Chatbot

A single-file Bitcoin chatbot — one `index.html`, no backend, no build step. Powered by the Anthropic API directly from the browser.

## Usage

1. Open `index.html` in any modern browser
2. Paste your Anthropic API key when prompted (get one at https://console.anthropic.com)
3. Ask Bitcoin questions

Your API key is stored in your browser's localStorage and never leaves your machine except to call the Anthropic API.

## Security note

This app uses Anthropic's direct-browser-access mode, which is intended for personal/local use only.

**Never deploy this publicly with a shared API key embedded** — anyone could read it from the page source and run up your bill. For public hosting, put a small server-side proxy in front of the API instead.

## Configuration

The model is set near the top of the script in `index.html` (currently `claude-sonnet-4-20250514`). If Anthropic retires that model, update the constant to a current one.

## License

MIT
