---
description: >
  Planeja estratégia de conteúdo com pilares, calendário editorial e abordagem
  por plataforma. Use quando pedirem plano de conteúdo, calendário de posts,
  estratégia de marketing, organização de conteúdo, ou planejamento editorial.
argument-hint: "[nicho] [plataformas] [frequência]"
---

# Planejamento de Estratégia de Conteúdo

## O que fazer

Crie um plano de conteúdo completo incluindo pilares, calendário editorial, funil de conteúdo e estratégia por plataforma.

## Etapa 1: Pilares de Conteúdo

Defina 3-5 pilares temáticos para a marca. Cada pilar deve:
- Ser relevante para o público-alvo
- Ter potencial de conteúdo recorrente
- Misturar educação, entretenimento e autoridade

**Exemplo para nicho "Marketing Digital":**
1. 🎯 **Estratégia** — Planejamento, funis, posicionamento
2. 📱 **Redes Sociais** — Dicas práticas, algoritmos, trends
3. 💡 **Cases e Resultados** — Estudos de caso, antes/depois
4. 🛠 **Ferramentas** — Reviews, tutoriais, hacks
5. 🧠 **Mindset** — Produtividade, rotina, bastidores

## Etapa 2: Funil de Conteúdo

### TOFU — Topo do Funil (Awareness) — 50% do conteúdo
- Trends, memes, conteúdo viral
- Posts educativos rápidos
- Reels com hooks fortes
- Objetivo: alcance e novos seguidores

### MOFU — Meio do Funil (Consideração) — 30% do conteúdo
- Carrosséis educativos aprofundados
- Vídeos de YouTube com tutoriais
- Stories com enquetes e interação
- Objetivo: engajamento e autoridade

### BOFU — Fundo do Funil (Conversão) — 20% do conteúdo
- Depoimentos e cases
- Ofertas e CTAs diretos
- Conteúdo exclusivo (isca para email/grupo)
- Objetivo: vendas e leads

## Etapa 3: Calendário Semanal

Consulte `templates/weekly-calendar.md` para o formato completo.

**Estrutura recomendada:**

| Dia | Formato | Pilar | Funil | Plataforma |
|-----|---------|-------|-------|------------|
| Seg | Carrossel educativo | [pilar] | MOFU | Instagram + LinkedIn |
| Ter | Reels/TikTok | [pilar] | TOFU | Instagram + TikTok |
| Qua | Post com dica rápida | [pilar] | TOFU | X + LinkedIn |
| Qui | Vídeo YouTube | [pilar] | MOFU | YouTube |
| Sex | Carrossel storytelling | [pilar] | MOFU | Instagram |
| Sáb | Conteúdo lifestyle/bastidores | [pilar] | TOFU | Stories |
| Dom | Conteúdo de valor + CTA | [pilar] | BOFU | Todas |

## Etapa 4: Estratégia por Plataforma

### Instagram
- **Frequência:** 4-7 posts/semana + stories diários
- **Mix:** 40% carrossel, 30% reels, 20% imagem, 10% collab
- **Melhor horário:** 11h-13h e 18h-21h
- **Hashtags:** 15-25 por post, mix de grande/médio/nicho

### TikTok
- **Frequência:** 1-3 vídeos/dia
- **Mix:** 60% trends, 30% educativo, 10% bastidores
- **Melhor horário:** 7h-9h, 12h-15h, 19h-23h
- **Duração ideal:** 15-30s para viralizar, 60s+ para autoridade

### YouTube
- **Frequência:** 1-2 vídeos/semana + 3-5 shorts
- **Mix:** 50% tutoriais, 30% análises, 20% vlogs
- **Melhor horário:** Qui-Sáb, 14h-16h
- **SEO:** Título, descrição, tags, timestamps, cards

### LinkedIn
- **Frequência:** 3-5 posts/semana
- **Mix:** 40% texto longo, 30% carrossel, 20% artigo, 10% vídeo
- **Melhor horário:** Ter-Qui, 8h-10h
- **Tom:** Profissional mas autêntico, storytelling pessoal

### X (Twitter)
- **Frequência:** 3-10 tweets/dia
- **Mix:** 50% thoughts/insights, 30% threads, 20% interação
- **Melhor horário:** 8h-10h, 12h-13h, 17h-18h

## Output

```
## Estratégia de Conteúdo: [marca/nicho]

### Persona
- **Nome:** [persona fictícia]
- **Idade:** [faixa]
- **Dores:** [lista de problemas]
- **Desejos:** [lista de objetivos]
- **Onde está:** [plataformas que usa]

### Pilares de Conteúdo
[lista dos 3-5 pilares com descrição]

### Tom de Voz
[descrição do tom: formal/informal, técnico/acessível, etc.]

### Calendário Semanal
[tabela com plano semanal]

### Calendário Mensal — [mês]
[4 semanas detalhadas com temas específicos]

### Métricas para Acompanhar
[KPIs por plataforma]
```

## Integrações

- Use `/viral-trends` para alinhar com tendências atuais
- Use `/viral-hooks` para gerar hooks dos posts planejados
- Use `/viral-carousel` para criar os carrosséis do calendário
- Use `/viral-reels` para roteirizar os vídeos curtos
- Se **Gamma MCP** disponível: criar a estratégia como apresentação visual
- Se **n8n MCP** disponível: criar workflow de automação para o calendário

## Parâmetros

- **nicho** (obrigatório): Nicho/área de atuação
- **plataformas** (opcional, default: instagram): instagram, tiktok, youtube, linkedin, x
- **frequência** (opcional, default: diário): diário, 3x-semana, semanal
- **objetivo** (opcional, default: crescimento): crescimento, engajamento, vendas, autoridade
- **idioma** (opcional, default: pt-br): pt-br, en, es
