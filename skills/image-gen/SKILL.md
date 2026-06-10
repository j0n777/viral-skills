---
description: >
  Gera imagens com IA para conteúdo de redes sociais. Cria thumbnails,
  imagens de carrossel, posts, backgrounds e arte visual. Use quando
  pedirem para gerar, criar ou fazer design de imagens para conteúdo.
argument-hint: "[descrição] [formato: 1:1|9:16|16:9]"
---

# Gerador de Imagens com IA

## O que fazer

Gere prompts otimizados para criação de imagens e, quando MCPs de design estiverem disponíveis, crie as imagens diretamente.

## Presets de Formato

| Uso | Dimensão | Aspect Ratio |
|-----|----------|--------------|
| Post Instagram | 1080x1080 | 1:1 |
| Carrossel Instagram | 1080x1350 | 4:5 |
| Story/Reels | 1080x1920 | 9:16 |
| Thumbnail YouTube | 1280x720 | 16:9 |
| Banner LinkedIn | 1584x396 | 4:1 |
| Post X/Twitter | 1200x675 | 16:9 |
| Cover Facebook | 820x312 | ~2.6:1 |

## Estilos Visuais

### Fotorrealista
- Prompt base: "professional photography, natural lighting, shallow depth of field, 8k"
- Ideal para: thumbnails, posts de lifestyle, produto

### 3D Render
- Prompt base: "3D render, volumetric lighting, octane render, clean background"
- Ideal para: thumbnails YouTube, posts tech, ilustrações

### Flat/Ilustração
- Prompt base: "flat illustration, vector style, clean lines, vibrant colors"
- Ideal para: carrosséis, infográficos, ícones

### Ghibli/Anime
- Prompt base: "studio ghibli style, soft pastel colors, dreamy atmosphere, watercolor"
- Ideal para: posts inspiracionais, storytelling visual

### Minimalista
- Prompt base: "minimalist design, lots of white space, single focal point, clean"
- Ideal para: quotes, dicas, posts elegantes

### Neon/Dark
- Prompt base: "dark background, neon glow, cyberpunk aesthetic, dramatic lighting"
- Ideal para: posts tech, music, nightlife

## Prompt Engineering

### Estrutura do prompt
```
[estilo] [sujeito principal] [ação/pose] [ambiente/fundo] [iluminação] [detalhes extras] [qualidade]
```

### Modificadores de qualidade
- `8k, ultra detailed, sharp focus` — para máxima qualidade
- `professional photography` — para fotorrealismo
- `award-winning` — para composição forte

### Negative prompts (o que evitar)
- `blurry, low quality, watermark, text, logo, ugly, deformed`

## Output

```
## Imagem: [descrição curta]

**Formato:** [dimensão e aspect ratio]
**Estilo:** [estilo visual]

### Prompt Principal
[prompt completo otimizado]

### Prompt Negativo
[negative prompt]

### Variações
1. [variação A do prompt]
2. [variação B do prompt]

### Instruções de uso
- [onde e como usar a imagem]
- [sugestão de texto overlay se aplicável]
```

## Integrações

- Se **Canva MCP** disponível: criar design direto via `mcp__Canva__generate-design`
- Para thumbnails: combinar com `/youtube-title-thumbnail`
- Para carrosséis: combinar com `/viral-carousel`

## Parâmetros

- **descrição** (obrigatório): O que a imagem deve mostrar
- **formato** (opcional, default: 1:1): 1:1, 4:5, 9:16, 16:9
- **estilo** (opcional, default: fotorrealista): fotorrealista, 3d, flat, ghibli, minimalista, neon
- **provider** (opcional, default: auto): ideogram, midjourney, dalle, flux
- **quantidade** (opcional, default: 1): Número de variações
