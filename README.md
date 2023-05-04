[![Author](https://img.shields.io/badge/Dev-Nadi%20Duno-blueviolet%20)](https://portfolio-nadi.vercel.app/)
[![Social](https://img.shields.io/twitter/follow/nadiduno?label=%40nadiduno&style=social)](https://twitter.com/nadiduno)
[![Linkedin](https://img.shields.io/badge/in-Nadi%20Duno-blue)](https://www.linkedin.com/in/nadiduno/)
<br />
<br />


# ChatGPTWhisperVoce
Um código para conversar por voz com o ChatGPT utilizando Whisper (OpenAI) e Python

![Language](https://img.shields.io/badge/%3C%2F%3E-language-lightgrey)<br/>
[Python](https://www.python.org/)

```python
import openai

# Configura a chave de API da OpenAI usando a variável de ambiente 'OPENAI_API_KEY'
openai.api_key = os.environ.get('OPENAI_API_KEY')

# Envia uma requisição à API do ChatCompletion usando o modelo GPT-3.5 Turbo
# Lembrando que, a variável 'transcription' contém a transcrição do nosso áudio.
response = openai.ChatCompletion.create(
    model="gpt-3.5-turbo",
    messages=[ { "role": "user", "content": transcription } ]
)

# Obtém a resposta gerada pelo ChatGPT
chatgpt_response = response.choices[0].message.content
print(chatgpt_response)
```

https://github.com/openai/whisper

Feito com <💜 /> DevRel [Nadi Duno](https://www.linkedin.com/in/nadiduno/) |  © 2023
