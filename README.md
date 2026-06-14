# Cantina del Nonno

Site institucional completo de um restaurante italiano fictício em Pinheiros, São Paulo — construído como projeto de aprendizado de HTML/CSS/JS.

## Como rodar localmente

Basta abrir o arquivo `index.html` diretamente no browser. Não há dependências, servidor ou build step — tudo roda no cliente.

```
Abra o Explorer → navegue até a pasta → duplo clique em index.html
```

## O que você vê

Hero em tela cheia com gradiente marrom-escuro e título serifado em itálico; cardápio com 12 pratos filtráveis por categoria (Antipasti, Pasta, Secondi, Dolci) em grid responsivo; formulário de reserva com validação, máscara de telefone e modal de confirmação. A seção de localização exibe mapa OpenStreetMap em duas colunas com endereço copiável, horários e botões de navegação (Google Maps / Waze). Botão flutuante de WhatsApp aparece após 300px de scroll.

## Tecnologias

| Camada | Tecnologia |
|--------|-----------|
| Markup | HTML5 semântico |
| Estilo | Tailwind CSS via CDN + CSS custom (IntersectionObserver, dark mode) |
| Lógica | JavaScript vanilla (ES5/ES6, sem frameworks) |
| Dados | `cardapio.json` (12 pratos estruturados) |
| Fontes | Google Fonts — Playfair Display + Inter |
| Mapa | OpenStreetMap embed (sem API key) |

## Arquivos

```
index.html      → página principal
cardapio.json   → dados do cardápio (12 pratos)
robots.txt      → permissões de crawl (SEO + bots de LLM)
llms.txt        → contexto canônico para LLMs (padrão llmstxt.org)
sitemap.xml     → índice de URLs para buscadores
```

## SEO & GEO

- Meta tags completas (title, description, canonical, keywords)
- Open Graph + Twitter Card
- Schema.org JSON-LD (`@type: Restaurant`) com endereço, geo, horários, cardápio
- `robots.txt` com permissão explícita para GPTBot, ClaudeBot, PerplexityBot, Google-Extended, CCBot e outros bots de LLM
- `llms.txt` seguindo o padrão [llmstxt.org](https://llmstxt.org)

## Licença

MIT — use, modifique e distribua livremente.
