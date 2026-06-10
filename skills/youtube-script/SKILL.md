---
description: >
  Gera roteiros completos de YouTube a partir de tema ou URL de vídeo.
  Cria scripts com hooks, capítulos, e técnicas de retenção. Use quando
  pedirem roteiro de YouTube, script de vídeo, ou quiserem repurposar conteúdo.
argument-hint: "[tema ou URL do YouTube]"
---

# Gerador de Roteiros de YouTube

## O que fazer

Gere um roteiro completo e otimizado para YouTube. Se receber uma URL, use WebFetch para extrair informações do vídeo e criar um roteiro melhorado ou complementar.

## Estrutura do Roteiro

### 1. Hook (0-30s)
- Abrir com declaração impactante ou pergunta
- Criar loop aberto: "Ao final desse vídeo você vai saber..."
- Referenciar o thumbnail/título (manter promessa)
- **Nunca** começar com "E aí pessoal" ou saudação genérica

### 2. Promessa + Credibilidade (30s-1min)
- Dizer exatamente o que a pessoa vai aprender
- Estabelecer autoridade rapidamente
- Pattern interrupt visual (B-roll, gráfico, meme)

### 3. Conteúdo Principal (1min-80%)
- Dividir em capítulos claros (3-7 seções)
- 1 pattern interrupt a cada 2-3 minutos (mudar ângulo, inserir gráfico, fazer pergunta)
- Usar storytelling dentro dos pontos técnicos
- Manter tensão: "mas o próximo ponto muda tudo..."

### 4. Clímax/Revelação (80%-90%)
- O ponto mais valioso do vídeo
- Cumprir a promessa do hook
- Momento "aha" claro

### 5. CTA + Teaser (últimos 10%)
- CTA: like, inscrever, comentar (1 principal)
- Teaser do próximo vídeo (criar antecipação)
- End screen com vídeos relacionados

## Técnicas de Retenção

- **Open Loop:** Criar curiosidade que só resolve mais tarde
- **Pattern Interrupt:** Mudar estímulo visual/auditivo a cada 2-3min
- **Bucket Brigade:** Frases de transição ("Mas tem mais...", "Aqui é onde fica interessante...")
- **Curiosity Gap:** Mencionar algo que será revelado depois
- **Social Proof:** Dados, cases, resultados dentro do conteúdo
- **Direct Address:** Falar diretamente com o espectador

## Output

```
## Roteiro: [título do vídeo]

**Duração estimada:** [X minutos]
**Público-alvo:** [descrição]
**Objetivo:** [informar/entreter/converter]

---

### HOOK (0:00 - 0:30)

[Texto completo do que falar, com indicações de visual entre colchetes]

[B-ROLL: descrição da imagem/vídeo de apoio]

---

### CAPÍTULO 1: [Título] (0:30 - X:XX)

[Texto completo...]

[GRÁFICO: descrição]
[PATTERN INTERRUPT: o que fazer]

---

### CAPÍTULO 2: [Título] (X:XX - X:XX)

[...]

---

### CTA + ENCERRAMENTO (X:XX - X:XX)

[Texto do CTA]
[ENDSCREEN: descrição]

---

## Metadados

**Título sugerido:** [título otimizado para CTR]
**Descrição:** [descrição com keywords SEO]
**Tags:** [lista de tags relevantes]
**Timestamps:**
- 0:00 [capítulo]
- X:XX [capítulo]
- ...

**Thumbnail concept:** [descrição do thumbnail ideal]
```

## Modo Análise (quando receber URL)

Se o input for uma URL do YouTube:
1. Usar WebFetch para acessar a página do vídeo
2. Extrair informações disponíveis (título, descrição, metadados)
3. Oferecer opções:
   - Reescrever o roteiro com melhorias
   - Criar versão condensada (Reels/Shorts)
   - Criar carrossel baseado no conteúdo
   - Criar roteiro de resposta/complemento

## Parâmetros

- **tema/url** (obrigatório): Tema do vídeo ou URL do YouTube
- **duração** (opcional, default: 10min): Duração alvo em minutos
- **estilo** (opcional, default: educativo): educativo, vlog, tutorial, react, análise, storytelling
- **idioma** (opcional, default: pt-br): pt-br, en, es
