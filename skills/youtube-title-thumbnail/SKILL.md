---
description: >
  Gera títulos otimizados para CTR e conceitos de thumbnail para YouTube.
  Use quando pedirem ideias de título, sugestões de thumbnail, otimização
  de CTR, ou como fazer um vídeo ser clicado.
argument-hint: "[tema ou URL do YouTube]"
---

# Gerador de Títulos e Thumbnails para YouTube

## O que fazer

Gere 10 variações de título ranqueadas por potencial de CTR e 3 conceitos de thumbnail detalhados.

## Fórmulas de Título (Alto CTR)

### Com Números
- "7 [coisas] que [resultado]"
- "Como [resultado] em [tempo específico]"
- "De [estado A] para [estado B] em [tempo]"

### Com Curiosidade
- "[Resultado incrível] (e como você também pode)"
- "Por que [coisa comum] é um [erro/mito]"
- "O que [pessoa famosa/empresa] não quer que você saiba sobre..."

### Com Emoção
- "Pare de [erro comum] AGORA (faça isso em vez)"
- "Eu [fiz algo arriscado] e isso aconteceu..."
- "[Resultado] que mudou minha vida"

### Com Urgência
- "Faça isso ANTES que seja tarde"
- "A [oportunidade] que vai acabar em [tempo]"
- "Se você não fizer isso agora, vai se arrepender"

### Com Autoridade
- "Depois de [X anos/projetos], aprendi que..."
- "[Expert] revela o segredo de..."
- "O método que [empresa/pessoa] usa para..."

## Regras de Título

- Max 60 caracteres (ideal: 40-55)
- Palavra-chave principal no início
- CAPS para 1-2 palavras de ênfase (não o título todo)
- Parênteses para contexto extra: "Como ganhar dinheiro (sem investir)"
- Evitar clickbait que não cumpre a promessa
- Testar legibilidade no mobile (texto menor)

## Conceito de Thumbnail

### Elementos que funcionam
- **Rosto com emoção:** Surpresa, choque, alegria exagerada
- **Texto curto:** Max 4-5 palavras, fonte bold
- **Contraste alto:** Cores vibrantes, fundo simples
- **Setas/círculos:** Direcionar atenção para elemento chave
- **Before/After:** Divisão visual clara
- **Números grandes:** "R$ 10.000" ou "300%" em destaque

### O que evitar
- Texto demais (se precisa ler, já perdeu)
- Imagens genéricas de banco
- Cores apagadas/sem contraste
- Repetir o título inteiro no thumbnail

## Output

```
## Títulos (ranqueados por potencial de CTR)

| # | Título | Fórmula | CTR Potencial | Por que funciona |
|---|--------|---------|---------------|------------------|
| 1 | [título] | [fórmula] | ⭐⭐⭐⭐⭐ | [explicação] |
| 2 | [título] | [fórmula] | ⭐⭐⭐⭐⭐ | [explicação] |
| ... | ... | ... | ... | ... |

## Thumbnails

### Conceito 1: [nome]
- **Composição:** [layout - onde fica cada elemento]
- **Texto overlay:** [palavras no thumbnail, max 4-5]
- **Expressão facial:** [que emoção mostrar]
- **Cores:** [paleta principal]
- **Fundo:** [descrição do background]
- **Prompt para IA:** [prompt para gerar com Ideogram/Midjourney/DALL-E]

### Conceito 2: [nome]
[...]

### Conceito 3: [nome]
[...]
```

## Integrações

- Se **Canva MCP** disponível: ofereça criar o thumbnail direto no Canva
- Se receber URL de vídeo existente: analisar thumbnail atual e sugerir melhorias

## Parâmetros

- **tema/url** (obrigatório): Tema do vídeo ou URL do YouTube
- **nicho** (opcional): Nicho do canal para contextualizar
- **estilo** (opcional, default: moderno): moderno, minimalista, bold, 3d
- **idioma** (opcional, default: pt-br): pt-br, en, es
