---
description: >
  Cria composições de vídeo usando IA. Gera vídeos com HeyGen HyperFrames,
  edita com Descript, ou cria prompts para Veo/Runway/Sora. Use quando
  pedirem para criar, editar ou compor um vídeo.
argument-hint: "[conceito] [duração] [formato: 16:9|9:16|1:1]"
---

# Criador de Vídeo com IA

## O que fazer

Crie composições de vídeo usando as ferramentas de IA disponíveis, ou gere briefs detalhados de produção quando MCPs não estiverem conectados.

## Workflow por MCP

### Com HeyGen HyperFrames MCP
1. Definir conceito e storyboard
2. Criar composição HTML animada via `mcp__HyperFrames_by_HeyGen__compose`
3. Revisar projeto via `mcp__HyperFrames_by_HeyGen__get_project`
4. Renderizar via `mcp__HyperFrames_by_HeyGen__render_video`
5. Acompanhar status via `mcp__HyperFrames_by_HeyGen__get_render_status`

### Com Descript MCP
1. Criar/encontrar projeto via `mcp__Descript__list_projects`
2. Importar mídia via `mcp__Descript__import_media`
3. Editar com IA via `mcp__Descript__prompt_project_agent`
4. Acompanhar jobs via `mcp__Descript__wait_for_job`

### Sem MCPs (modo brief)
Gerar documentação completa de produção que pode ser executada manualmente.

## Formatos de Vídeo

| Tipo | Dimensão | Duração | Plataforma |
|------|----------|---------|------------|
| Reels/TikTok | 1080x1920 (9:16) | 15-90s | Instagram, TikTok |
| YouTube | 1920x1080 (16:9) | 3-15min | YouTube |
| Shorts | 1080x1920 (9:16) | 15-60s | YouTube |
| Stories | 1080x1920 (9:16) | 15s | Instagram |
| Feed Square | 1080x1080 (1:1) | 15-60s | Instagram, LinkedIn |

## Tipos de Composição

### Text Animation
- Texto animado com transições
- Ideal para: quotes, dicas, listas
- Técnica: motion graphics, kinetic typography

### Slideshow
- Sequência de imagens com transições
- Ideal para: antes/depois, portfolio, timeline
- Técnica: fade, slide, zoom transitions

### Talking Head + B-Roll
- Apresentador + imagens de apoio
- Ideal para: tutoriais, vlogs, reviews
- Técnica: cortes entre câmera e B-roll

### Screen Recording + Narração
- Gravação de tela com voz over
- Ideal para: tutoriais tech, demos, walkthroughs
- Técnica: zoom em áreas de foco, cursor highlight

## Output

```
## Brief de Vídeo: [título]

**Formato:** [dimensão]
**Duração:** [tempo]
**Tipo:** [composição]
**Plataforma:** [onde publicar]

### Storyboard

| Cena | Tempo | Visual | Áudio/Narração | Texto na tela |
|------|-------|--------|-----------------|---------------|
| 1 | 0-3s | [descrição] | [fala] | [overlay] |
| 2 | 3-8s | [descrição] | [fala] | [overlay] |
| ... | ... | ... | ... | ... |

### Especificações Técnicas
- **Resolução:** [dimensão]
- **FPS:** [24/30/60]
- **Formato de saída:** [MP4/MOV/WebM]
- **Música:** [tipo/mood]
- **Transições:** [tipo]

### Prompts para IA de Vídeo (se aplicável)
**Veo/Runway:** [prompt]
**Sora:** [prompt]

### Assets necessários
- [lista de imagens, sons, fontes necessárias]
```

## Parâmetros

- **conceito** (obrigatório): Ideia/tema do vídeo
- **duração** (opcional, default: 30s): Duração alvo
- **formato** (opcional, default: 9:16): 16:9, 9:16, 1:1
- **tipo** (opcional, default: auto): text-animation, slideshow, talking-head, screen-recording
- **plataforma** (opcional, default: reels): reels, youtube, tiktok, shorts, stories
