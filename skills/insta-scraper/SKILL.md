---
description: >
  Scraping de conteúdo viral e top vídeos do Instagram. Analisa posts de
  alto engajamento, padrões de conteúdo e estratégias de concorrentes.
  Use quando pedirem pesquisar Instagram, analisar concorrentes, encontrar
  posts virais, ou scraping de conteúdo.
argument-hint: "[username ou hashtag]"
---

# Scraper de Instagram

## O que fazer

Pesquise e analise conteúdo de alto desempenho no Instagram para um perfil ou hashtag específica.

## Modos de Operação

### Modo Script (quando scripts disponíveis)

Se os scripts Python estiverem configurados em `scripts/`:

```bash
# Scraping de conteúdo viral de um perfil
python3 scripts/scrape_viral.py --username [perfil] --limit 50

# Top vídeos de uma hashtag
python3 scripts/scrape_top_videos.py --hashtag [hashtag] --limit 30
```

**Requisitos:**
- `INSTAGRAM_SESSION_ID` configurado nas env vars
- Python 3.9+ com dependências instaladas

### Modo WebSearch (fallback)

Quando scripts não estiverem disponíveis, usar WebSearch para pesquisar:
- "[perfil] instagram viral posts"
- "top instagram posts [hashtag] [mês] [ano]"
- "[nicho] instagram content strategy analysis"
- "instagram [perfil] engagement rate"

## Análise Pós-Scraping

Para cada post/vídeo encontrado, analisar:

```
### Post [número]

**Tipo:** [carrossel/reels/imagem/story]
**Engajamento:** [likes/comments estimados]
**Hook:** [primeira frase da caption]
**Formato:** [educativo/entretenimento/inspiração/venda]
**Por que funcionou:** [análise do gatilho viral]
**Como adaptar:** [sugestão de conteúdo inspirado]
```

## Output

```
## Análise Instagram: @[perfil] ou #[hashtag]

### Resumo
- **Total analisado:** [X posts]
- **Período:** [datas]
- **Engajamento médio:** [média]

### Top 5 Posts por Engajamento
[lista dos 5 melhores com análise]

### Padrões Identificados
- **Melhor formato:** [carrossel/reels/etc]
- **Melhor horário:** [horários com mais engajamento]
- **Hooks mais usados:** [padrões de abertura]
- **Hashtags recorrentes:** [lista]
- **CTA mais eficaz:** [padrão de CTA]

### Estratégias do Perfil
1. [estratégia identificada]
2. [...]

### Recomendações
1. [ação baseada na análise]
2. [...]

### Ideias de Conteúdo (baseadas nos top posts)
1. [ideia inspirada no post X]
2. [...]
```

## Integrações

- Alimentar `/viral-hooks` com hooks que já funcionam no nicho
- Alimentar `/viral-carousel` com formatos que performam bem
- Combinar com `/viral-trends` para contexto de tendências

## Parâmetros

- **target** (obrigatório): Username (@perfil) ou hashtag (#hashtag)
- **limite** (opcional, default: 30): Número de posts para analisar
- **período** (opcional, default: 30 dias): Período de análise
- **foco** (opcional, default: completo): viral, reels, carrossel, estratégia

## Status

⚠️ **Scripts Python pendentes** — os scripts de `insta-viralscrap` e `insta-topvideos` serão portados em sessão separada. Enquanto isso, o modo WebSearch está funcional.
