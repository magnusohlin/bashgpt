# ʕ·ᴥ·ʔ BashGPT

![bashgpt](https://user-images.githubusercontent.com/521837/225560741-9872664c-d483-416a-888e-096970e33ceb.png)

BashGPT is a simple command-line interface to interact with OpenAI's GPT-3.5-turbo model. It allows users to chat with the model directly from their terminal and even open the latest response in Vim for further editing.

## Prerequisites

1. `curl`: A command-line tool for transferring data with URLs.
2. `jq`: A lightweight and flexible command-line JSON processor.
3. An OpenAI API key

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

3.  Move it to a directory that is already in your PATH or add the file to your system's `PATH`. This can be done by adding the following line to your `.bashrc` or `.zshrc`:

```
export PATH=$PATH:/path/to/directory/containing/gpt
```
4. Set your OpenAI API key as an environment variable OPENAI_API_KEY in your shell or in your `.bashrc` or `.zshrc` file:

```
export OPENAI_API_KEY="your_api_key_here"
```

## Usage

To start using BashGPT, open your terminal and type:

```
gpt
```

You will be greeted with a welcome message and an input prompt. Type your questions or prompts and press Enter to receive a response from GPT-3.5-turbo. To open the latest response in Vim, type "vi" at the prompt. The script will then exit after opening Vim.

If you prefer to provide the API key as a command-line argument instead of using the environment variable, you can use the -k option:

```
gpt -k your_api_key_here
```

## License

This project is licensed under the MIT License.
