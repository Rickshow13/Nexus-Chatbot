# 🤖 NEXUS — Assistente Inteligente

NEXUS é um chatbot de IA feito para ajudar em estudos: dicas de organização, técnicas de foco e memória, planos de estudo personalizados e explicações didáticas sobre qualquer assunto — tudo em Português Brasileiro.

Todo o projeto roda em um **único arquivo HTML**, sem servidor próprio, sem instalação e sem custo. Basta abrir a página e conversar.

## ✨ Funcionalidades

- Chat com IA (modelo `openai/gpt-oss-120b` via [Groq Cloud](https://groq.com), gratuito)
- Atalhos rápidos para os temas mais comuns (dicas de estudo, concentração, memória, gestão de tempo, plano de estudos, curiosidades)
- **Histórico de conversas**: salva várias conversas no navegador e permite reabrir qualquer uma delas depois
- Cada pessoa usa sua própria chave da Groq — guardada só no navegador dela, nunca em um servidor
- Interface responsiva, funciona em celular, tablet e computador
- Visual futurista com mascote animado em SVG

## 🚀 Como usar

1. Acesse a página publicada (link no topo do repositório, se estiver no GitHub Pages) ou abra o arquivo `index.html` direto no navegador
2. Na primeira vez, crie uma chave gratuita em [console.groq.com/keys](https://console.groq.com/keys) (não pede cartão de crédito, leva menos de 1 minuto)
3. Cole a chave na tela inicial do NEXUS e comece a conversar

## 🛠 Tecnologias

- HTML5, CSS3 e JavaScript puro (sem frameworks, sem dependências além das fontes do Google)
- [Groq Cloud API](https://groq.com) — inferência rápida com o modelo `openai/gpt-oss-120b`
- `localStorage` do navegador para guardar chave e histórico de conversas localmente

## 💻 Rodando localmente

Não precisa de instalação. Basta baixar o repositório e abrir o `index.html`:

```bash
git clone https://github.com/Rickshow13/nexus-chatbot.git
cd nexus-chatbot
```

Depois é só abrir o `index.html` no navegador (duplo clique ou arrastar para a janela do navegador).

## 🌐 Publicando no GitHub Pages

1. Vá em **Settings → Pages** neste repositório
2. Em "Source", selecione a branch `main` e a pasta `/root`
3. Salve — em 1-2 minutos o link fica disponível em `https://<seu-usuário>.github.io/<nome-do-repositório>`

## 🔒 Segurança e privacidade

- A chave de API de cada pessoa é salva **somente no navegador dela** (`localStorage`) — nunca é enviada para nenhum servidor além da própria Groq
- O histórico de conversas também fica salvo localmente no navegador, não em nenhum servidor externo
- Como é 100% front-end, não existe banco de dados nem backend guardando informações de ninguém

## ⚠️ Limitações conhecidas

- A conta gratuita da Groq tem um limite de mensagens por minuto por chave — em uso intenso, pode ser necessário aguardar alguns segundos entre mensagens
- O histórico fica salvo no navegador local; trocar de dispositivo ou navegador não traz as conversas antigas junto
- As respostas são geradas por IA e podem conter erros — sempre vale conferir informações importantes

## 📌 Próximos passos (ideias)

- Exportar conversas em PDF
- Suporte a múltiplos idiomas
- Tela de configuração para trocar o modelo de IA usado

## 👤 Autor

Desenvolvido por **Henrique** ([@Rickshow13](https://github.com/Rickshow13)).

## 📄 Licença

Este projeto é de uso livre para fins educacionais.
