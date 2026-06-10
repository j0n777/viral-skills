---
description: >
  Gera roteiros para vídeos curtos — Reels, TikTok, YouTube Shorts.
  Cria hook, corpo e CTA com timing e direção visual. Use quando pedirem
  roteiro de reels, script de TikTok, ideia de vídeo curto, ou short.
argument-hint: "[tema] [duração: 15s|30s|60s|90s]"
---

# Gerador de Roteiros para Vídeos Curtos

## O que fazer

Gere um roteiro completo para vídeo curto com timing preciso, texto falado, direção visual e sugestões de edição.

## Estrutura por Duração

### 15 segundos
- 0-3s: Hook (parar o scroll)
- 3-10s: Conteúdo principal (1 ideia só)
- 10-15s: CTA rápido

### 30 segundos
- 0-3s: Hook
- 3-8s: Contexto/problema
- 8-22s: Conteúdo/solução
- 22-27s: Resultado/prova
- 27-30s: CTA

### 60 segundos
- 0-3s: Hook visual + verbal
- 3-10s: Setup do problema
- 10-35s: Desenvolvimento (2-3 pontos)
- 35-50s: Solução/revelação
- 50-57s: Resultado/transformação
- 57-60s: CTA

### 90 segundos
- 0-5s: Hook forte
- 5-15s: Contexto e promessa
- 15-60s: Conteúdo principal (3-5 pontos com pattern interrupts)
- 60-80s: Conclusão/revelação
- 80-90s: CTA duplo (seguir + salvar)

## Formatos Trending

### POV (Point of View)
- "POV: você descobriu que [situação]"
- Câmera fixa ou selfie
- Reação no rosto é essencial

### Storytime
- "Essa história é real..."
- Narração pessoal com cortes rápidos
- Plot twist no final

### Coisas que ninguém te conta
- Lista format com text-on-screen
- Transições rápidas entre itens
- Reação surpresa no final

### Before/After
- Divisão clara visual
- Transformação impactante
- Música que acompanha a revelação

### Tutorial Rápido
- "Como fazer X em Y segundos"
- Mãos na câmera / screen recording
- Steps claros com números na tela

## Output

```
## Roteiro: [título do vídeo]

**Duração:** [Xs]
**Formato:** [formato trending]
**Plataforma:** [reels/tiktok/shorts]

### Timeline

| Tempo | Fala/Narração | Visual/Câmera | Texto na tela | Áudio |
|-------|---------------|---------------|---------------|-------|
| 0-3s  | [texto]       | [direção]     | [overlay]     | [som] |
| ...   | ...           | ...           | ...           | ...   |

### Elementos de Produção
- **Câmera:** [selfie/tripé/mão/drone]
- **Iluminação:** [natural/ring light/golden hour]
- **Edição:** [cortes rápidos/smooth transitions/jump cuts]
- **Música sugerida:** [tipo de música/mood]

### Caption
[Legenda do post com hashtags]

### Hooks Alternativos
1. [variação de hook 1]
2. [variação de hook 2]
3. [variação de hook 3]
```

## Integrações

- Se **HeyGen HyperFrames MCP** disponível: ofereça criar composição visual com `mcp__HyperFrames_by_HeyGen__compose`
- Se **Descript MCP** disponível: ofereça criar projeto no Descript com `mcp__Descript__import_media`

## Parâmetros

- **tema** (obrigatório): Assunto do vídeo
- **duração** (opcional, default: 30s): 15s, 30s, 60s, 90s
- **formato** (opcional, default: auto): pov, storytime, tutorial, before-after, lista
- **plataforma** (opcional, default: reels): reels, tiktok, shorts
- **idioma** (opcional, default: pt-br): pt-br, en, es
