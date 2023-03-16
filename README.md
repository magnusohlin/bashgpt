# BashGPT

BashGPT is a simple command-line interface to interact with OpenAI's GPT-3.5-turbo model. It allows users to chat with the model directly from their terminal and even open the latest response in Vim for further editing.

## Prerequisites

1. `curl`: A command-line tool for transferring data with URLs.
2. `jq`: A lightweight and flexible command-line JSON processor.

Install them using package managers like `apt`, `brew`, or `yum`. For example:

```
sudo apt install curl jq
```

## Setup

1. Save the provided script as a file named `gpt` in your desired directory.
2. Make the file executable by running the following command:

```
chmod +x gpt
```

3. Add the file to your system's `PATH`. This can be done by adding the following line to your `.bashrc` or `.zshrc`:

```
export PATH=$PATH:/path/to/directory/containing/gpt
```

4. Replace the `API_KEY` value with your OpenAI API key:

```
API_KEY="your_openai_api_key"
```

## Usage

To start using BashGPT, open your terminal and type:

```
gpt
```

You will be greeted with a welcome message and an input prompt. Type your questions or prompts and press Enter to receive a response from GPT-3.5-turbo. To open the latest response in Vim, type "vi" at the prompt. The script will then exit after opening Vim.

## License

This project is licensed under the MIT License.
