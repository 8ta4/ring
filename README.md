# shock

## Shock Some Sense into It

> What is this tool about?

`shock` rates phrases for shock value.

## Setup

> How do I set up `shock`?

1. Make sure you're using a Mac with Apple silicon.

1. Make sure the billing account linked to your Google AI Studio project is on Tier 2.

1. Install [Homebrew](https://brew.sh/#install).

1. Install [devenv](https://github.com/cachix/devenv/blob/83e8d7d34bdebad98ab936b6af53d57ae67af420/docs/src/getting-started.md#installation).

1. Open a terminal.

1. Copy an API key from [Google AI Studio](https://aistudio.google.com/api-keys).

1. Run these commands:
   ```bash
   mkdir -p ~/.config/shock
   pbpaste > ~/.config/shock/key
   git clone https://github.com/8ta4/shock
   cd shock
   devenv allow
   devenv shell download
   ```

## Usage

> How do I run `shock`?

1. Open a terminal.

1. Run the command with an attribute.

   ```bash
   sense negative
   ```

Once the API batches finish, `shock` will drop two files into your current directory:

- negative.tsv: a file that contains normalized scores

- negative.json: a file that contains raw scores

