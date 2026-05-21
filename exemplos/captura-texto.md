# Exemplo de captura — só texto

Este exemplo mostra como a skill processa uma captura simples, só texto, sem imagem. Serve de referência prática pra quem (humano ou assistente) quiser ver a gramática funcionando.

---

## Input do Pedro

> "hoje vi um pássaro no parque do meu prédio. Branco, andando devagar na grama molhada. Fiquei parado uns dois minutos olhando."

Mensagem solta, no celular, no fim da tarde. Sem imagem. Sem comando explícito — só o registro.

## Leitura da skill

**Verbo de entrada:** *vi*, *fiquei parado olhando* → sinaliza Galeria de Hator (paisagem, beleza, gesto observado).

**Sujeito:** Pássaro (animal observado em ambiente urbano) → reforça Hator.

**Tom emocional:** awe leve (medo+surpresa) — o silêncio do passo do passro, a interrupção do tempo. Tag: `emocao/admiracao`.

**Ligação simbólica óbvia:** Íbis, que também é um passaro, é o animal-totem do Pedro. Menção é justa. Não inventada.

**Densidade:** média. Merece pergunta de releitura.

## Output gerado

**Nome do arquivo:** `ibis-parque-2026-05-21.md`

**Salvo em:** `Nun/`

**Conteúdo da nota:**

```markdown
---
criado: 21/05/2026 às 17:42
sala: A Galeria de Hator
tags: [emocao/admiracao, passaro, parque, manha-lenta]
estado: semente
companhia: sozinho
lugar: parque do prédio
humor: 
---

*21/05/2026 — 17:42*

---

# O Pássaro no parque hoje

Branca. Andando devagar na grama molhada. Parei dois minutos.

Tinha um silêncio do tipo que se ouve. O passo dela era preciso — sem pressa, sem ansiedade. Como se o parque fosse dela e eu o visitante.

Coincidência ou não, **a íbis é meu animal-totem**. Não tinha pensado nisso ali, no momento. Só agora, escrevendo, é que volto e vejo o gesto do encontro.

---

> O que você reconheceu nela que te fez parar?

→ [[Parou o Olhar]] · [[íbis]] (criar?) · [[A Galeria de Hator]]
```

## Resposta da skill pro Pedro

> Guardado em Nun como `passaro-parque-2026-05-21.md`. Sugeri [[A Galeria de Hator]]. Quer ajustar?

## Notas sobre escolhas feitas

- **Título "O Pássaro no parque hoje"** — frase, não etiqueta. Carrega o tempo (*hoje*) que vai virar passado quando ele reler dali a um ano. O "hoje" envelhece bonito.
- **Primeiro parágrafo quase intocado.** Pedro escreveu "Branco, andando devagar na grama molhada. Fiquei parado uns dois minutos olhando." A skill manteve as três frases, só ajustou cadência em "Parei dois minutos" (mais ritmo curto).
- **Segundo parágrafo elabora atmosfera.** "Silêncio do tipo que se ouve" e "passo preciso" não são fato novo — são leitura do que Pedro descreveu. Usa vocabulário dele (precisão, sem pressa, sem ansiedade).
- **Terceiro parágrafo faz a ligação simbólica** — só porque íbis é totem dele. Se fosse pomba ou pardal, a skill teria parado no segundo parágrafo.
- **Negrito numa palavra-chave:** *animal-totem*. Não em "íbis" porque ela já aparece muito; o negrito vai na palavra que carrega o vinco simbólico.
- **Pergunta de releitura:** abre uma porta sem responder. "O que você reconheceu nela" é mais útil que "como você se sentiu" — convida ele a pensar no que da íbis ressoou, não a auto-diagnosticar emoção.
- **Link `[[animal totem]] (criar?)`:** indica nota-conceito potencial. Se Pedro tiver outras capturas com animais-totem, virar nota-conceito faz sentido. A skill marca a possibilidade sem decidir.
- **`humor:` vazio:** Pedro não disse o humor geral do dia. Skill não inventa. O campo fica como convite pra ele preencher depois.

## O que esta captura NÃO faz

- Não vira mood tracker — a tag emocional é uma só, precisa, sem pedir escala.
- Não pede confirmação a cada decisão — só uma linha no fim, perguntando se quer ajustar.
- Não usa H2 nem H3 — a nota é curta, prosa primeiro.
- Não usa emoji decorativo — os emojis do vault moram nos nomes das salas.
- Não enche de tags — 5 tags é suficiente.
- Não faz Pedro responder a pergunta de releitura agora — ela espera pelo retorno futuro.
