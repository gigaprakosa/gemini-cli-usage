# Gemini Usage

A lightweight CLI tool to aggregate and display token usage statistics from your Gemini CLI sessions.

## Overview

Gemini Usage scans your local Gemini CLI session logs to provide a clear summary of token consumption and estimated costs. It aggregates data by month and presents it in a clean, readable format directly in your terminal.

## Features

- **Automatic Discovery:** Automatically locates session logs in the default Gemini CLI directory.
- **Monthly Aggregation:** Groups token usage by month for easy tracking.
- **Cost Estimation:** Provides cost estimates based on standard token pricing.
- **Model Breakdown:** Tracks usage across different Gemini models used in your sessions.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/gemini-usage.git
   cd gemini-usage
   ```

2. Make the script executable:
   ```bash
   chmod +x gemini-usage
   ```

3. (Optional) Add an alias to your shell profile (e.g., `~/.zshrc` or `~/.bashrc`) for easier access:
   ```bash
   echo "alias gemini-usage='$(pwd)/gemini-usage'" >> ~/.zshrc
   source ~/.zshrc
   ```

## Usage

Simply run the command from your terminal:

```bash
gemini-usage
```

### Example Output

```text
📊 Gemini CLI Usage (last 2 months):
• 2026-04: 7,436,411 tokens, Cost: $22.61
• 2026-05: 60,803,167 tokens, Cost: $183.69
```

## Contributing

Contributions are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details.

## License

This project is licensed under the [MIT License](LICENSE).
