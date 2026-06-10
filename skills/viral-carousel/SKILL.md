---
description: >
  Cria carrosséis para Instagram, LinkedIn ou TikTok. Gera textos slide-a-slide,
  instruções de design, e prompts de imagem. Use quando pedirem carrossel,
  slides, post de arrastar, conteúdo multi-imagem, ou swipe post.
argument-hint: "[tema] [template: educativo|storytelling|lista|bible] [slides]"
---

# Gerador de Carrosséis Virais

## O que fazer

Gere um carrossel completo com texto para cada slide, incluindo instruções visuais e prompt de imagem para cada um.

## Estrutura do Carrossel

Todo carrossel segue esta anatomia:

1. **Slide 1 — Cover (Hook):** Título impactante que para o scroll. Máximo 8 palavras. Design chamativo.
2. **Slides 2 a N-1 — Conteúdo:** Informação valiosa, 1 ideia por slide. Máximo 40 palavras por slide.
3. **Slide N — CTA:** Call-to-action claro. Perfil, convite para seguir, salvar, ou comentar.

## Templates Disponíveis

Consulte os arquivos em `templates/` para detalhes de cada formato:

### Educativo (`templates/educational.md`)
- Formato: Problema → Explicação → Solução → Aplicação
- Ideal para: dicas, tutoriais, how-to
- Slides recomendados: 7-10

### Storytelling (`templates/storytelling.md`)
- Formato: Situação → Conflito → Virada → Lição
- Ideal para: cases, experiências pessoais, transformações
- Slides recomendados: 5-8

### Lista/Dicas (`templates/listicle.md`)
- Formato: 1 dica por slide com ícone/número
- Ideal para: "5 dicas para...", "7 erros que...", "10 ferramentas..."
- Slides recomendados: 7-12

### Bíblico (`templates/bible.md`)
- Formato: Versículo → Contexto → Reflexão → Aplicação → Oração
- Ideal para: devocionais, estudos, inspiração
- Slides recomendados: 5-7

## Regras de Design

### Texto
- Máximo 40 palavras por slide (exceto cover que é max 8)
- Fonte grande e legível (mínimo 24pt equivalente)
- Contraste alto entre texto e fundo
- Hierarquia visual clara (título > subtítulo > corpo)

### Visual
- Formato: 1080x1350px (4:5) para Instagram, 1080x1080 para LinkedIn
- Paleta de cores consistente em todos os slides
- Elementos visuais repetidos (ícones, linhas, formas) para unidade

### Estilos visuais
- **Moderno:** Gradientes, sans-serif, cores vibrantes
- **Minimalista:** Fundo branco/claro, tipografia forte, espaço negativo
- **Dark:** Fundo escuro, texto claro, neon accents
- **Ghibli:** Ilustrações suaves, tons pastéis, storytelling visual
- **Foto:** Imagem de fundo com overlay escuro + texto branco

## Output

Para cada slide, forneça:

```
### Slide [número] — [tipo: Cover/Conteúdo/CTA]

**Texto principal:** [texto do slide]
**Texto secundário:** [subtítulo ou complemento, se houver]
**Instrução visual:** [descrição do layout e elementos visuais]
**Prompt de imagem:** [prompt para gerar o fundo/ilustração com IA]
**Cores:** [cores principais do slide]
```

Após todos os slides, inclua:

```
### Caption do Post
[Legenda completa para o post com hashtags]
```

## Integrações

- Se **Canva MCP** disponível: ofereça criar o design direto no Canva usando `mcp__Canva__generate-design`
- Se **Gamma MCP** disponível: ofereça criar como apresentação visual via Gamma

## Parâmetros

- **tema** (obrigatório): Assunto do carrossel
- **template** (opcional, default: educativo): educativo, storytelling, lista, bible
- **slides** (opcional, default: 7): Número de slides (5-12)
- **estilo** (opcional, default: moderno): moderno, minimalista, dark, ghibli, foto
- **plataforma** (opcional, default: instagram): instagram, linkedin, tiktok
- **idioma** (opcional, default: pt-br): pt-br, en, es
