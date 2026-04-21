# CodeAnalytics-AI
## ⚠️ Observação  Este bot funciona apenas enquanto o script estiver rodando localmente no terminal. Para mantê-lo online 24/7, é necessário eu hospedá-lo em um servidor, pretendo fazer isso futuramente.

# 🤖 GitHub Analytics Bot

Bot do Telegram que analisa repositórios do GitHub usando Inteligência Artificial e retorna um relatório completo com métricas e insights do projeto.

## 📸 Demo

![Demo do bot](<img width="1224" height="915" alt="portfoliogithubbot" src="https://github.com/user-attachments/assets/63dde44a-2d6c-424e-9e16-cbbb4641732e" />)

## 💡 Sobre o projeto

O GitHub Analytics Bot permite analisar qualquer repositório público do GitHub diretamente pelo Telegram. Basta enviar o comando `/repo` com o nome do repositório e o bot busca as métricas na API do GitHub e gera uma análise completa usando o modelo Llama 3.3 da Groq.

## ✨ Funcionalidades

- Busca automática de métricas do repositório via API do GitHub
- Análise gerada por IA (Llama 3.3 70B via Groq)
- Exibe stars, forks, issues abertas, contribuidores e linguagem principal
- Identifica pontos positivos, riscos e sugere melhorias
- Feedback visual de carregamento enquanto analisa
- Tratamento de erros amigável para o usuário

## 🛠️ Tecnologias utilizadas

- [Python 3](https://www.python.org/)
- [python-telegram-bot](https://github.com/python-telegram-bot/python-telegram-bot)
- [Groq API](https://console.groq.com) — modelo Llama 3.3 70B
- [GitHub REST API](https://docs.github.com/en/rest)

## ⚙️ Como rodar localmente

### Pré-requisitos

- Python 3.10 ou superior
- Conta no [Telegram](https://telegram.org)
- Conta no [Groq](https://console.groq.com)
- Conta no [GitHub](https://github.com)

### Instalação

1. Clone o repositório
```bash
git clone https://github.com/davidi0358/analytics-github-bot.git
cd analytics-github-bot
```

2. Instale as dependências
```bash
pip install python-telegram-bot groq requests urllib3
```

3. Configure as variáveis no arquivo `analytics_github.py`

| Variável | Onde obter |
|---|---|
| `TELEGRAM_TOKEN` | [@BotFather](https://t.me/BotFather) no Telegram |
| `GROQ_API_KEY` | [console.groq.com](https://console.groq.com) |
| `GITHUB_TOKEN` | [github.com/settings/tokens](https://github.com/settings/tokens) |

4. Rode o bot
```bash
python3 analytics_github.py
```

## 📱 Como usar

No Telegram, encontre seu bot e envie:

```
/start
```
```
/repo torvalds/linux
```
```
/repo microsoft/vscode
```
