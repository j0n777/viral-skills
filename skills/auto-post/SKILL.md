---
description: >
  Automação e agendamento de posts. Cria calendários de publicação,
  gera conteúdo em batch, e configura workflows de automação. Use quando
  pedirem agendar posts, automatizar publicação, criar pipeline de
  conteúdo, ou batch content.
argument-hint: "[plataforma] [frequência]"
---

# Automação de Posts

## O que fazer

Configure pipelines de automação para publicação de conteúdo, incluindo geração em batch, agendamento e workflows automatizados.

## Funcionalidades

### 1. Batch Content Generation
Gere conteúdo para múltiplos dias de uma vez:
- 7 dias de posts (1 semana)
- 30 dias de posts (1 mês)
- Mix de formatos (carrossel, reels, imagem, texto)

### 2. Calendário de Publicação
Defina horários ótimos por plataforma:

| Plataforma | Melhores Horários | Melhores Dias |
|------------|-------------------|---------------|
| Instagram | 11h-13h, 18h-21h | Ter, Qui, Sáb |
| TikTok | 7h-9h, 12h-15h, 19h-23h | Todos |
| YouTube | 14h-16h | Qui, Sex, Sáb |
| LinkedIn | 8h-10h | Ter, Qua, Qui |
| X | 8h-10h, 12h-13h | Seg-Sex |

### 3. Workflows de Automação

#### Com n8n MCP (quando disponível)
Criar workflows automatizados via `mcp__n8n__create_workflow_from_code`:

- **Auto-post schedule:** Trigger por horário → gerar conteúdo → postar
- **Content pipeline:** Ideia → gerar hook → gerar carrossel → agendar
- **Trend-to-content:** Monitorar trends → criar conteúdo relevante → postar
- **Repurpose pipeline:** Vídeo YouTube → extrair → criar reels + carrossel + tweets

#### Sem n8n (modo manual)
Gerar todo o conteúdo organizado por data/horário para publicação manual.

## Output

```
## Plano de Automação: [período]

### Configuração
- **Plataformas:** [lista]
- **Frequência:** [posts/dia por plataforma]
- **Período:** [datas]

### Conteúdo Gerado

#### Semana 1

| Data | Horário | Plataforma | Formato | Conteúdo | Status |
|------|---------|------------|---------|----------|--------|
| [data] | [hora] | Instagram | Carrossel | [link/resumo] | 📝 Rascunho |
| [data] | [hora] | TikTok | Reels | [link/resumo] | 📝 Rascunho |
| ... | ... | ... | ... | ... | ... |

### Workflow n8n (se aplicável)
[código do workflow ou link]

### Checklist de Setup
- [ ] Configurar env vars de APIs
- [ ] Testar conexão com plataformas
- [ ] Aprovar conteúdo da primeira semana
- [ ] Ativar workflow/agendamento
```

## Integrações

- `/viral-hooks` → gerar hooks para os posts
- `/viral-carousel` → gerar carrosséis do calendário
- `/viral-reels` → roteirizar vídeos agendados
- `/viral-trends` → alinhar conteúdo com trends atuais
- `/cross-post` → adaptar e publicar em múltiplas redes
- **n8n MCP** → criar workflows automatizados

## Parâmetros

- **plataformas** (obrigatório): Onde publicar
- **frequência** (obrigatório): Posts por dia/semana
- **período** (opcional, default: 7 dias): Período do batch
- **nicho** (opcional): Nicho para contextualizar conteúdo
- **pilares** (opcional): Pilares de conteúdo definidos

## Status

⚠️ **Scripts de automação pendentes** — código do autoposter será portado em sessão separada. Skills de planejamento e geração de batch já funcionam.
