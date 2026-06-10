---
description: >
  Gera conteúdo bíblico para redes sociais. Cria devocionais, carrosséis
  de versículos, roteiros de vídeos inspiracionais e posts de fé.
  Use quando pedirem conteúdo bíblico, devocional, versículo do dia,
  estudo bíblico para redes, ou conteúdo cristão.
argument-hint: "[tema ou referência bíblica]"
---

# Gerador de Conteúdo Bíblico

## O que fazer

Gere conteúdo de fé para redes sociais, combinando profundidade teológica com formato viral. O conteúdo deve ser acessível, respeitoso e biblicamente fundamentado.

## Tipos de Conteúdo

### 1. Devocional Diário
- 1 versículo em destaque
- Contexto breve (2-3 frases)
- Reflexão prática para o dia
- Oração curta (3-4 linhas)
- Formato: imagem com versículo + caption

### 2. Carrossel Devocional
- Use `/viral-carousel` com template `bible`
- 5-7 slides: versículo → contexto → significado → aplicação → oração → CTA
- Design clean, cores quentes, tipografia elegante

### 3. Estudo Temático (Série)
Temas populares para séries de conteúdo:
- **Fé e Confiança:** Hebreus 11, Salmo 23, Provérbios 3:5-6
- **Gratidão:** Salmo 100, 1 Tessalonicenses 5:18, Colossenses 3:17
- **Coragem:** Josué 1:9, Isaías 41:10, 2 Timóteo 1:7
- **Família:** Salmo 127, Provérbios 22:6, Efésios 6:1-4
- **Provisão:** Mateus 6:25-34, Filipenses 4:19, Salmo 37:25
- **Propósito:** Jeremias 29:11, Romanos 8:28, Efésios 2:10
- **Amor:** 1 Coríntios 13, João 3:16, 1 João 4:7-8
- **Sabedoria:** Provérbios 4:7, Tiago 1:5, Salmo 111:10
- **Paz:** João 14:27, Filipenses 4:6-7, Isaías 26:3
- **Cura:** Salmo 147:3, Isaías 53:5, Jeremias 17:14

### 4. Histórias Bíblicas em Formato Viral
Recontar histórias bíblicas em linguagem moderna:
- Formato storytelling para carrossel
- Roteiro de reels narrativo
- Thread estilo "você sabia que..."

### 5. Promessas de Deus
- Versículos de promessa com design impactante
- Formato: 1 versículo por imagem
- Série: "7 dias de promessas sobre [tema]"

### 6. Reels Devocional
- Use `/viral-reels` com tema bíblico
- 30-60s com narração + versículo na tela
- Música suave de fundo
- Hook: "Deus tem uma palavra pra você hoje..."

## Traduções Bíblicas

Usar preferencialmente:
- **NVI** (Nova Versão Internacional) — linguagem acessível
- **NVT** (Nova Versão Transformadora) — muito moderna
- **ARA** (Almeida Revista e Atualizada) — tradicional respeitada
- **NTLH** (Nova Tradução na Linguagem de Hoje) — muito simples

Sempre indicar a tradução usada: `"Texto do versículo" (Livro X:Y, NVI)`

## Regras Importantes

- SEMPRE citar referência completa (livro, capítulo, versículo)
- NUNCA tirar versículo do contexto para mudar o significado
- Respeitar o contexto histórico e cultural
- Tom acolhedor, não condenatório
- Acessível para quem não conhece a Bíblia
- Incluir aplicação prática (não só teoria)
- Evitar polêmicas denominacionais

## Calendário Litúrgico

Alinhar conteúdo com datas importantes:
- **Natal** (Dez) — Advento, nascimento de Jesus
- **Páscoa** (Mar/Abr) — Quaresma, ressurreição
- **Dia das Mães/Pais** — Família na Bíblia
- **Ano Novo** — Renovação, propósito
- **Semana Santa** — Via crucis, reflexão

## Output

```
## Conteúdo Bíblico: [tema/versículo]

### Versículo Principal
"[texto do versículo]" ([referência], [tradução])

### Contexto
[quem escreveu, quando, para quem, situação]

### Reflexão
[aplicação prática para hoje, 3-5 frases]

### Oração
[oração curta baseada no versículo]

### Formatos de Conteúdo

**Para Carrossel:**
[estrutura dos slides — usar /viral-carousel template bible]

**Para Reels:**
[roteiro curto — usar /viral-reels]

**Para Post Imagem:**
[texto do versículo formatado + caption]

### Caption
[legenda do post com hashtags: #fé #devocional #versículododia etc.]
```

## Integrações

- `/viral-carousel` com template `bible` → carrosséis devocionais
- `/viral-reels` → roteiros de vídeos devocionais
- `/image-gen` estilo minimalista → imagens com versículos
- `/content-strategy` → planejamento de séries bíblicas

## Parâmetros

- **tema/referência** (obrigatório): Tema (ex: "fé") ou referência bíblica (ex: "João 3:16")
- **tipo** (opcional, default: devocional): devocional, estudo, história, promessa, série
- **formato** (opcional, default: todos): carrossel, reels, imagem, texto
- **tradução** (opcional, default: NVI): NVI, NVT, ARA, NTLH
- **idioma** (opcional, default: pt-br): pt-br, en, es
