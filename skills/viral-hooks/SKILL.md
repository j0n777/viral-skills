---
description: >
  Gera hooks virais para redes sociais. Use quando pedirem hooks, aberturas,
  frases de impacto, scroll-stoppers, ou chamadas de atenção para qualquer
  plataforma (Instagram, TikTok, YouTube, X, LinkedIn).
argument-hint: "[tema] [plataforma] [estilo]"
---

# Gerador de Hooks Virais

## O que fazer

Gere hooks virais baseados no tema fornecido. Cada hook deve parar o scroll e criar curiosidade imediata.

## Frameworks de Hook

Use estas fórmulas comprovadas, variando entre elas:

1. **Curiosity Gap** — "A maioria das pessoas não sabe que..."
2. **Contrarian** — "Pare de fazer X (faça isso em vez)"
3. **Social Proof** — "Como X pessoas conseguiram Y em Z dias"
4. **Shocking Stat** — "97% das pessoas erram isso sobre..."
5. **Story Hook** — "Eu perdi tudo até descobrir que..."
6. **FOMO** — "Se você não fizer isso agora, vai perder..."
7. **Direct Challenge** — "Aposto que você não sabia disso sobre..."
8. **Question Hook** — "Por que ninguém fala sobre...?"
9. **Authority** — "Depois de 10 anos fazendo X, aprendi que..."
10. **Listicle** — "5 coisas que [pessoa bem-sucedida] faz todo dia"

## Regras por Plataforma

### Instagram
- Primeiras 5 palavras são cruciais (aparecem no preview)
- Max 2200 chars na caption, mas hook precisa ter < 125 chars
- Emojis estratégicos (1-2 no hook)
- CTA no final: "Salve para não esquecer" / "Manda pra alguém que precisa"

### TikTok
- Primeiros 3 segundos = tudo. Hook deve ser falado em até 3s
- Tom conversacional e direto
- Padrão: "POV:", "Coisas que ninguém te conta sobre..."
- Sem hashtags no hook (vão na descrição)

### YouTube
- Hook = primeiros 30 segundos do vídeo
- Criar loop aberto: "Ao final desse vídeo você vai saber..."
- Incluir promessa específica e mensurável
- Referenciar o thumbnail no hook

### X (Twitter)
- Max 280 caracteres
- Tom provocativo ou surpreendente
- Sem emojis excessivos (1 max)
- Thread hook: primeira frase precisa ser autossuficiente

### LinkedIn
- Tom profissional mas humano
- Storytelling pessoal funciona melhor
- Primeira linha com quebra de expectativa
- Evitar clickbait extremo (audiência julga)

## Output

Para cada hook gerado, inclua:

```
## Hook [número]

**Tipo:** [framework usado]
**Plataforma ideal:** [onde funciona melhor]
**Hook:** [o texto do hook]
**Por que funciona:** [1 frase explicando o gatilho mental]
**Sugestão de CTA:** [call to action complementar]
```

## Parâmetros

- **tema** (obrigatório): O assunto do conteúdo
- **plataforma** (opcional, default: todas): instagram, tiktok, youtube, x, linkedin
- **estilo** (opcional, default: mix): polêmico, educativo, storytelling, humorístico, autoridade
- **quantidade** (opcional, default: 10): Número de hooks
- **idioma** (opcional, default: pt-br): pt-br, en, es

## Exemplos

Entrada: `/viral-hooks "marketing digital" instagram educativo`

Saída esperada: 10 hooks educativos sobre marketing digital otimizados para Instagram.
