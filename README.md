

# AI Tools for chatGPT

> This cli tool allows you to easily use chatGPT in the terminal. You can chat with it, have it answer questions for you, or even translate text. 
And it supports rendering Markdown in the terminal.

[中文](README.zh.md) | [English](README.md) | [日本語](README.ja.md)

## Quick Start (No Installation Needed)

```bash
curl https://raw.githubusercontent.com/yufeikang/ai-cli/main/ai.py -L -s | python - ask "Hello"
```

## Installation

```bash
curl https://raw.githubusercontent.com/yufeikang/ai-cli/main/ai.py -L -s> /usr/local/bin/ai && chmod +x /usr/local/bin/ai && pip install -U rich 
openai
```

## Usage

Ask questions

```bash
ai ask "Hello"
# no stream mode
ai --no-stream ask "Hello"
# help
ai ask --help
```

![](./_/video/ask.gif)

Translate

```bash
ai translate "Hello"
ai translate "Hello" -t japanese
ai translate -t english -f "file.txt"
echo "Hello" | ai translate -t english
cat "file.txt" | ai translate -t english
```

![](./_/video/translate.gif)

Chat

```bash
ai chat
```

![](./_/video/chat.gif)

## Dependencies

```bash
pip install rich openai
```