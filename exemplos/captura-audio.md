# Exemplo de captura — áudio

Este exemplo mostra como a skill processa uma captura que vem com áudio (gravação de fala, música ouvida, voz nota, som ambiente). A diferença essencial em relação a texto e imagem: no áudio, o **conteúdo dito** e o **efeito sonoro/atravessamento emocional** são duas camadas distintas — e a skill precisa ser clara sobre qual está lendo a cada momento.

A distinção decide a sala:

- Foco no **conteúdo dito** (que ideias, frases, narrativa foi falada) → Alexandria (ideia), Ganesha (análise se for obra), Pomar (se foi pessoa importante falando).
- Foco no **efeito sonoro / tom de voz / atravessamento** (como soou, como atravessou) → Vozes (gosto/atravessamento estético) ou Afetos (reação interna direta).

Quando as duas camadas existem com peso parecido, a skill marca uma como principal e a outra no corpo da nota.

---

## Input do Pedro

Pedro envia um arquivo de áudio (`voz-nota.m4a`, 47 segundos) com a seguinte mensagem:

> "ouvi essa fala do Caetano agora. cara, a voz dele caindo nessa última frase me derrubou. ele tá dizendo uma coisa sobre saudade que eu já sabia, mas a forma como ele diz é que pegou."

A skill recebe o áudio e a mensagem juntos.

## Leitura da skill

**Duas camadas presentes:**

- **Conteúdo dito:** Caetano fala sobre saudade. Pedro reconhece que a *ideia* não é nova ("já sabia").
- **Efeito / atravessamento:** a *forma* como Caetano diz — a voz caindo na última frase — é o que pegou Pedro. Isso é o foco.

**Decisão de foco:** o atravessamento sonoro é o que ele está marcando, não a ideia. Pedro foi explícito: "a forma como ele diz é que pegou".

**Sala principal:** A Câmara das Vozes (atravessamento estético, voz como obra).

**Sala secundária possível:** A Sala dos Afetos (a reação interna — "me derrubou" — é direta e corpórea). Marcar no corpo.

**Tags emocionais:** atravessamento + algo entre awe e melancolia (a voz caindo evoca queda, descida, fim). Tags: `emocao/awe`, `emocao/melancolia`.

**Áudio:** salvo em `Nun/_anexos/caetano-saudade-2026-05-22-01.m4a`. Renderizado inline na nota com Obsidian audio embed.

## Output gerado

**Nome do arquivo:** `caetano-saudade-2026-05-22.md`

**Salvo em:** `Nun/`

**Áudio salvo em:** `Nun/_anexos/caetano-saudade-2026-05-22-01.m4a`

**Conteúdo da nota:**

```markdown
---
criado: 22/05/2026 às 14:08
sala: A Câmara das Vozes
tags: [emocao/awe, emocao/melancolia, voz, caetano, saudade, queda, atravessamento]
estado: semente
companhia: sozinho
lugar: 
humor: atravessado
---

*22/05/2026 — 14:08*

---

# A voz dele caindo na última frase

![[caetano-saudade-2026-05-22-01.m4a]]

> Ouvi essa fala do Caetano agora. A voz dele caindo nessa última frase me derrubou. Ele tá dizendo uma coisa sobre saudade que eu já sabia, mas a forma como ele diz é que pegou.

A ideia não é nova — Caetano fala sobre saudade como muitos já falaram. O que abriu o chão foi a **descida** da voz na última frase. Como se ela soubesse o que estava dizendo antes da palavra terminar.

A voz não ilustrou o conceito. Ela foi o conceito.

*Talvez também more em [[A Sala dos Afetos]] — o "me derrubou" é reação interna direta, não só leitura estética.*

---

> O que você reconhece nessa queda de voz que faz a ideia ganhar peso só ali?

→ [[Chamados]] · [[voz como obra]] (criar?) · [[A Câmara das Vozes]] · [[A Sala dos Afetos]]
```

## Resposta da skill pro Pedro

> Guardado em Nun como `caetano-saudade-2026-05-22.md`, com o áudio anexo (47s). Foco em Vozes pelo atravessamento sonoro; marquei Afetos como segunda casa possível. Quer ajustar?

## Notas sobre escolhas feitas

### Sobre as duas camadas (conteúdo vs atravessamento)

- **Conteúdo dito** ("ideia sobre saudade") é mencionado mas não é o foco da nota. Pedro mesmo disse que já conhecia. A skill **não** elabora a ideia — não cabe inventar o que Caetano disse e teorizar. Respeita o que Pedro marcou: o atravessamento.
- **Atravessamento** (voz caindo, "me derrubou", forma > conteúdo) vira o centro da elaboração. Os dois parágrafos de prosa giram em torno disso. A frase "A voz não ilustrou o conceito. Ela foi o conceito." é vinco curto pra fechar a tensão entre conteúdo e forma.

### Sobre o áudio como anexo

- **Pasta:** `Nun/_anexos/` — mesma das imagens. Anexo é anexo.
- **Nome:** `caetano-saudade-2026-05-22-01.m4a` — slug + data + sufixo `-01`. Se viessem três áudios diferentes na mesma captura, seriam `-01`, `-02`, `-03`.
- **Sintaxe Obsidian:** `![[arquivo.m4a]]` — sem alt text, porque Obsidian renderiza player inline. Áudio é ouvido, não descrito. (Diferente de imagem, onde alt text protege contra perda visual.)
- **Posicionamento:** após o H1, antes da fala citada. O player vira porta de entrada pra revisita: Pedro reabre a nota, dá play, e o atravessamento volta.

### Sobre a citação em bloco

- A fala original do Pedro entra em `>` (callout de citação) logo após o player. Isso separa visualmente o que ele *disse* do que a skill *elaborou*. Marca duas vozes na mesma página.
- Sem alteração no que ele escreveu além de capitalizar a primeira letra. Voz dele preservada.

### Sobre marcar sala alternativa no corpo

- A frase em itálico `*Talvez também more em [[A Sala dos Afetos]]...*` aparece antes da pergunta de releitura. Marca a segunda casa possível sem competir com a principal. Pedro decide no Scriptorium se quer mover, ligar ou deixar.

### Sobre tags emocionais combinadas

- `emocao/awe` (medo + surpresa) + `emocao/melancolia` (tristeza leve) — combinação que faz sentido pra "queda de voz que abre o chão". Não é só admiração nem só tristeza; é a combinação que carrega o momento.

### Sobre `lugar:` vazio

- Pedro não disse onde estava. A skill não inventa. O campo fica como convite pra ele preencher depois, se a memória do lugar voltar.

### Sobre `humor: atravessado`

- A palavra "derrubou" autoriza "atravessado". A skill propõe, não impõe; Pedro corrige se errou.

## Variações do mesmo tipo de captura

A regra de duas camadas vale também pra:

- **Música ouvida** — conteúdo (letra, narrativa) vs efeito (melodia, arranjo, voz). Em geral, música vai pra Vozes; se a letra disparou ideia que ganhou vida própria, vai pra Alexandria.
- **Voz nota de amigo** — conteúdo (o que ele disse) vs tom (como ele estava, audível na voz). Pode ir pra Pomar (pessoa) com tag de `voz` se o tom importou.
- **Podcast / fala de terceiros** — conteúdo (a ideia exposta) vs forma (como o convidado expôs). Pode ir pra Alexandria (ideia) ou Vozes (atravessamento).
- **Som ambiente** (chuva, pássaros, barulho urbano) — geralmente Hator (paisagem sonora) ou Afetos (se o som mexeu com humor diretamente).
- **Áudio próprio** (Pedro falando consigo) — vai pra Maat (se reconheceu padrão), Alexandria (se foi ideia em voz alta), Afetos (se foi desabafo), ou Toth (se foi rascunho de criação).

## O que esta captura faz que as anteriores não faziam

- Trata anexo de áudio (player inline, sem alt text).
- Trabalha explicitamente com duas camadas (conteúdo vs forma).
- Usa citação em bloco (`>`) pra separar voz de Pedro da voz da skill.
- Marca sala alternativa no corpo, demonstrando o uso documentado em `salas-pistas.md`.
- Mostra que a skill respeita o foco que Pedro deu — se ele disse "a forma é que pegou", o foco vai pra forma, não pra conteúdo.

## O que esta captura NÃO faz

- Não transcreve o áudio inteiro no corpo da nota. O áudio fica como anexo audível; transcrição vai só se Pedro pedir explicitamente (em modo Scriptorium, por exemplo, pra criar nota-conceito sobre o tema).
- Não teoriza sobre o conteúdo que o Caetano disse. Pedro não pediu análise da ideia; a skill respeita.
- Não força encaixe numa sala só. Marca a alternativa quando duas casas legitimam a captura.
- Não usa H2 — a nota é curta, prosa primeiro.
