# Gemini CLI Usage

A lightweight, zero-dependency CLI tool to aggregate and display token usage and cost statistics from your local Gemini CLI sessions.

## Overview

Gemini CLI Usage scans your local Gemini CLI session logs to provide a definitive summary of token consumption and estimated costs. It features a "Smart Pricing Engine" that automatically stays up-to-date with the latest Google API rates.

## Features

- **Smart Pricing Engine:** Automatically fetches the latest pricing data from the community-standard [LiteLLM database](https://github.com/BerriAI/litellm).
- **100% Data Accuracy:** Tracks all token types, including standard input/output, thought tokens (reasoning), cached context, and tool-generated tokens.
- **Advanced Billing Rules:** Correctly applies Gemini 3.1 billing nuances (e.g., thought tokens at output rates, discounted cache reads).
- **Automatic Discovery:** Seamlessly locates session logs in the default Gemini CLI directory.
- **Zero Dependencies:** Pure Python 3 using only the standard library for maximum portability and security.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/gigaprakosa/gemini-cli-usage.git
   cd gemini-cli-usage
   ```

2. Make the script executable:
   ```bash
   chmod +x gemini-cli-usage
   ```

3. (Optional) Add an alias to your shell profile (e.g., `~/.zshrc` or `~/.bashrc`) for easier access:
   ```bash
   echo "alias gemini-cli-usage='$(pwd)/gemini-cli-usage'" >> ~/.zshrc
   source ~/.zshrc
   ```

## Usage

Simply run the command from your terminal:

```bash
gemini-cli-usage
```

### Example Output

```text
📊 Gemini CLI Usage (last 2 months):
• 2026-04: 7,436,411 tokens, Cost: $2.72
• 2026-05: 86,282,310 tokens, Cost: $32.50
```

## Contributing

Contributions are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details.

## License

This project is licensed under the [MIT License](LICENSE).
