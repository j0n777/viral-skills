---
description: >
  Analisa canais e vídeos do YouTube. Avalia performance, identifica padrões
  de sucesso e sugere melhorias. Use quando pedirem análise de canal, análise
  de vídeo, competitor analysis, ou entender o que funciona no YouTube.
argument-hint: "[URL do canal ou vídeo]"
---

# Analisador de YouTube

## O que fazer

Analise um canal ou vídeo do YouTube identificando padrões de sucesso, oportunidades e recomendações práticas.

## Análise de Vídeo Individual

Ao receber URL de um vídeo, analise:

### Performance
- Proporção views/inscritos (virality ratio)
- Engajamento (likes/comments vs views)
- Retenção estimada (baseada em duração e tema)

### Conteúdo
- Eficácia do hook (primeiros 30s)
- Estrutura do roteiro
- Técnicas de retenção usadas
- Qualidade do CTA

### SEO
- Otimização do título (keywords, comprimento, fórmula)
- Descrição (keywords, links, timestamps)
- Tags e categorização
- Thumbnail (análise visual se possível)

### Potencial Viral
- Shareability (as pessoas vão compartilhar?)
- Comentabilidade (gera discussão?)
- Rewatchability (vale assistir de novo?)
- Search demand (as pessoas buscam isso?)

## Análise de Canal

Ao receber URL de canal, analise:

### Overview
- Nicho e posicionamento
- Frequência de publicação
- Crescimento estimado
- Pontos fortes e fracos

### Content Strategy
- Tipos de vídeo que performam melhor
- Padrões de título e thumbnail
- Duração ideal para o canal
- Temas com mais engajamento

### Oportunidades
- Content gaps (temas não explorados)
- Formatos não testados
- Colaborações potenciais
- Shorts/vídeos curtos

## Output

```
## Análise: [nome do canal/vídeo]

### Resumo Executivo
[2-3 frases com a principal conclusão]

### Pontos Fortes
1. [ponto forte com exemplo]
2. [...]

### Oportunidades de Melhoria
1. [melhoria com ação específica]
2. [...]

### Recomendações (próximos 30 dias)
1. [ação concreta e mensurável]
2. [...]

### Benchmark
- **Performance atual:** [nota de 1-10]
- **Potencial estimado:** [onde pode chegar]
- **Competidores para estudar:** [3 canais referência]
```

## Parâmetros

- **url** (obrigatório): URL do canal ou vídeo do YouTube
- **foco** (opcional, default: completa): performance, conteúdo, seo, estratégia
- **idioma** (opcional, default: pt-br): pt-br, en, es
