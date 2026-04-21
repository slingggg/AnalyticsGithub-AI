# 🤖 CodeAnalytics-AI

Bot do Telegram que analisa repositórios do GitHub usando Inteligência Artificial e retorna um relatório completo com métricas e insights do projeto.

## 📸 Preview

<p align="center">
  <img width="1224" height="730" src="https://github.com/user-attachments/assets/dff6f36a-a2bb-4866-a25e-017478d4d749" />
  <br><br>
  <img width="1224" height="915" src="https://github.com/user-attachments/assets/8fea8f47-97c6-4f06-b684-75efc214dc18" />
</p>

## 💡 Sobre o projeto

O GitHub Analytics Bot permite analisar qualquer repositório público do GitHub diretamente pelo Telegram. Basta enviar o comando `/repo` com o nome do repositório e o bot busca as métricas na API do GitHub, por exemplo /repo nome de usuario/nome do repositorio, e assim gera uma análise completa usando o modelo Llama 3.3 da Groq.

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
| `TELEGRAM_TOKEN` | Pesquise [@BotFather](https://t.me/BotFather) no Telegram |
| `GROQ_API_KEY` | Crie uma API Key: [console.groq.com](https://console.groq.com) |
| `GITHUB_TOKEN` | Crie um Token: [github.com/settings/tokens](https://github.com/settings/tokens) |

4. Rode o bot no terminal
```bash
python3 analytics_github.py
```

## 📱 Como usar

No Telegram, encontre seu bot e envie:

```
/start
```
```
/repo nome de usuario/nome do repositório
```

## 💡 Exemplo:

```
/repo davidi0358/CodeAnalytics-AI
```
## ⚠️ Este bot funciona apenas enquanto o código estiver rodando localmente no terminal. Para mantê-lo online 24/7, é necessário hospedá-lo em um servidor.

> **Segurança:** Nunca compartilhe seus tokens e chaves de API publicamente.
> Cada usuário deve criar e utilizar suas **próprias credenciais**.
> O nome do bot pode ser personalizado durante a criação no [@BotFather](https://t.me/BotFather).

## 👤 Autor

Feito por **david0358**

[![GitHub](https://img.shields.io/badge/GitHub-davidi0358-181717?style=flat&logo=github)](https://github.com/davidi0358)
[![Discord](https://img.shields.io/badge/Discord-5865F2?style=flat&logo=discord&logoColor=white)](https://discord.com/users/753736601523454063)

---
⭐ Se este projeto te ajudou, deixe uma estrela no repositório! **Obrigado**
