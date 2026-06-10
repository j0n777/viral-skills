---
description: >
  Cross-posting de conteúdo para múltiplas plataformas. Adapta formato e
  tom para cada rede. Suporta Instagram, X, Threads, LinkedIn, Telegram,
  Facebook e Discord. Use quando pedirem publicar em várias redes,
  cross-post, distribuir conteúdo, ou postar em múltiplas plataformas.
argument-hint: "[plataformas: instagram,x,threads,linkedin,telegram,discord]"
---

# Cross-Posting Multi-Plataforma

## O que fazer

Adapte e formate conteúdo para publicação em múltiplas plataformas, respeitando as regras e melhores práticas de cada uma.

## Adaptação por Plataforma

### Instagram
- **Caption:** Até 2200 chars, storytelling, emojis estratégicos
- **Hashtags:** 15-25 no final ou primeiro comentário
- **CTA:** "Salve", "Manda pra alguém", "Comenta"
- **Media:** 1080x1080 (feed), 1080x1350 (carrossel), 1080x1920 (stories/reels)

### X (Twitter)
- **Texto:** Max 280 chars, direto e provocativo
- **Hashtags:** 1-3 máximo, integradas no texto
- **Thread:** Se conteúdo longo, dividir em thread (1/ 2/ 3/)
- **Media:** 1200x675 ou 1200x1200
- **Tom:** Conversacional, opinativo, witty

### Threads
- **Texto:** Sem limite, mas posts curtos performam melhor
- **Hashtags:** Poucas ou nenhuma (algoritmo não depende)
- **Tom:** Casual, conversacional, sem formalidade
- **Media:** Similar ao Instagram

### LinkedIn
- **Texto:** Até 3000 chars, profissional mas pessoal
- **Hashtags:** 3-5, relevantes ao nicho profissional
- **Formato:** Texto longo com line breaks (hook na primeira linha)
- **Media:** 1200x627 (link), 1080x1080 (imagem)
- **Tom:** Autoridade + vulnerabilidade, cases com dados

### Telegram
- **Texto:** Markdown formatado, sem limite
- **Formato:** Post com botões inline (quando via bot)
- **Media:** Qualquer formato, preview de links
- **Tom:** Informativo, direto, newsletter-style

### Facebook
- **Texto:** Até 63,206 chars, mas 40-80 palavras ideal
- **Hashtags:** 1-2 ou nenhuma
- **Media:** 1200x630 (link), 1200x1200 (imagem)
- **Tom:** Comunidade, perguntas, compartilhável

### Discord
- **Texto:** Markdown/embeds formatados
- **Formato:** Embeds com cores, campos, imagens
- **Media:** Qualquer formato
- **Tom:** Comunidade, informal

## Workflow

1. Receber conteúdo original
2. Identificar plataformas alvo
3. Adaptar texto, tom e formato para cada uma
4. Ajustar media (dimensões, aspect ratio)
5. Gerar UTM links diferentes por plataforma (para tracking)
6. Apresentar preview de cada versão
7. Se script disponível, executar publicação

### Modo Script (quando disponível)
```bash
python3 scripts/post.py --platforms "instagram,x,threads" --content "texto" --media "imagem.jpg"
```

**Requisitos de env vars:**
- `TWITTER_API_KEY`, `TWITTER_API_SECRET`
- `TELEGRAM_BOT_TOKEN`
- `THREADS_ACCESS_TOKEN`
- `DISCORD_WEBHOOK_URL`

## Output

```
## Cross-Post: [título do conteúdo]

### Conteúdo Original
[conteúdo base]

---

### 📸 Instagram
**Caption:**
[texto adaptado com emojis e hashtags]

**Media:** [formato e dimensão]
**Melhor horário:** [sugestão]

---

### 🐦 X (Twitter)
**Tweet:**
[texto max 280 chars]

**Thread (se necessário):**
1/ [parte 1]
2/ [parte 2]

---

### 🔗 LinkedIn
**Post:**
[texto adaptado tom profissional]

---

[... para cada plataforma selecionada]

### 📊 Tracking
| Plataforma | UTM Link |
|------------|----------|
| Instagram | [utm_source=instagram] |
| X | [utm_source=twitter] |
| ... | ... |
```

## Parâmetros

- **conteúdo** (obrigatório): Texto/conteúdo a ser distribuído
- **plataformas** (obrigatório): Lista de plataformas alvo
- **media** (opcional): Caminho para imagem/vídeo
- **agendar** (opcional): Horário para publicação
- **utm** (opcional, default: sim): Gerar UTM tracking links

## Status

⚠️ **Script de publicação pendente** — o código do CrossPostrAI será portado em sessão separada. Enquanto isso, a skill gera o conteúdo adaptado para cada plataforma (copiar/colar manual).
