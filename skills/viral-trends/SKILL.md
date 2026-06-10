---
description: >
  Detecta tendências virais em tempo real nas redes sociais. Encontra trends,
  hashtags, formatos e sons que estão viralizado. Use quando pedirem trends,
  o que está viral, ideias baseadas em tendências, ou pesquisa de mercado.
argument-hint: "[plataforma] [nicho]"
---

# Detector de Tendências Virais

## O que fazer

Pesquise tendências atuais usando WebSearch e analise o potencial de cada uma para criação de conteúdo.

## Fontes de Pesquisa

Use WebSearch para buscar em:

### Por Plataforma
- **Instagram:** "instagram trends [nicho] [mês] [ano]", "viral reels [nicho]"
- **TikTok:** "tiktok trends today", "trending tiktok sounds [mês]", "tiktok [nicho] viral"
- **YouTube:** "youtube trending [país]", "youtube shorts trends [nicho]"
- **X/Twitter:** "twitter trending topics [região]", "viral tweets [nicho]"
- **LinkedIn:** "linkedin viral posts [nicho]", "linkedin content trends"

### Por Tipo
- **Formatos:** "trending content formats social media [ano]"
- **Áudios:** "trending sounds reels tiktok [mês] [ano]"
- **Hashtags:** "trending hashtags [plataforma] [nicho]"
- **Memes:** "viral memes [mês] [ano]"

## Análise de Cada Trend

Para cada tendência encontrada, avaliar:

```
### Trend: [nome/descrição]

**Plataforma:** [onde está trending]
**Tipo:** [formato/áudio/hashtag/meme/tema]
**Fase:** [🟢 crescendo | 🟡 pico | 🔴 declinando]
**Janela de oportunidade:** [quanto tempo ainda vale entrar]
**Dificuldade:** [fácil/médio/difícil de produzir]

**Como usar:**
1. [ângulo de conteúdo 1]
2. [ângulo de conteúdo 2]
3. [ângulo de conteúdo 3]

**Exemplo de referência:** [link ou descrição de quem fez bem]
```

## Output

```
## Tendências Virais — [data]

### 🔥 Trends Quentes (entrar AGORA)
[trends em fase de crescimento com alta oportunidade]

### 📈 Trends em Alta (próximos dias)
[trends com potencial mas ainda sem saturação]

### 💡 Oportunidades de Nicho
[trends específicas para o nicho do usuário]

### ⚠️ Trends Saturadas (evitar)
[trends que já passaram do pico]

---

### Plano de Ação Sugerido
1. [conteúdo prioritário baseado nas trends]
2. [segundo conteúdo]
3. [terceiro conteúdo]
```

## Integrações

- Se **LunarCrush MCP** disponível: usar para dados de social engagement
- Combinar com `/viral-hooks` para gerar hooks baseados nas trends
- Combinar com `/viral-carousel` ou `/viral-reels` para criar conteúdo baseado nas trends

## Parâmetros

- **plataforma** (opcional, default: todas): instagram, tiktok, youtube, x, linkedin
- **nicho** (obrigatório): Área de atuação para filtrar trends relevantes
- **região** (opcional, default: brasil): brasil, eua, global
- **idioma** (opcional, default: pt-br): pt-br, en, es
