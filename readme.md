# DeepSeek Chat CLI

A command-line chat tool based on DeepSeek API, supporting streaming responses and translation features.

version: 0.1.0

## Features

- Interactive chat, supports multi-line input, so you can input **your code** or other **multi-line text** in command line.
- Streaming response (use `stream#` prefix)
- Chinese-English translation (use `translate#` prefix)
- Balance query (type `balance`)
- Clear screen (type `clear`)
- Markdown formatted output rendering

## Installation
- must install rich and deepseek library first
```bash
pip install rich deepseek
```
## Configuration
- Configure API Key in my_key_dk.ini
```ini
[DeepSeek]
api_key=your_api_key
```
## Usage
1. Ensure the correct API Key is confiured in my_key_dk.ini.
2. Run the script:
```bash
python deepseek_chat.py
```
3. Start chatting!
4. input your message in command line, and the input supports multiple lines, press ":::" to end input.

## Commands
- Normal char:Directy input content
- stream#:Start streaming response
- translate#:Translate content to English
- balance:Check balance
- clear:Clear screen
- exit:Exit the chat
## Example
```bash
exit
:::

trans# 你好
:::

Please analyze the following text and provide a summary in Chinese:
[you can paste your text here]
:::
```

## Notes
1. Ensure stable network connection.
2. API Key needs to be configured correctly.
3. Translation feature is based on predefined system prompt.
4. Output uses rich library to render Markdown format.
## License
This project is licensed under the MIT License - see the LICENSE file for details.