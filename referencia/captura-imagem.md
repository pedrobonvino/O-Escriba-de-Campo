# Exemplo de captura — com imagem

Este exemplo mostra como a skill processa uma captura que vem com foto. Demonstra: salvamento da imagem como anexo, alt text descritivo, posicionamento no corpo, descrição atmosférica do que a skill viu (sem repetir o que Pedro já disse), e referência Obsidian correta.

---

## Input do Pedro

> "essa luz na cozinha agora cedo. tomei meu café aqui ouvindo a chuva começar lá fora."

Junto: uma foto da cozinha de manhã. Luz dourada baixa entrando pela janela, vapor saindo de uma xícara escura sobre a bancada, lá fora vidro embaçado, sinal de chuva fina.

Mensagem solta, no celular, manhã cedo. Captura com peso afetivo claro (luz + café + chuva — combinação que prende).

## Leitura da skill

**Verbo de entrada:** *tomei*, mas o verbo dominante implícito é *vi/reparei* (a foto fala por si). → Galeria de Hator.

**Sujeito:** luz na cozinha, café, chuva → cena cotidiana com peso estético. Hator confirmado.

**Tom emocional:** serenidade (alegria leve) + uma camada de melancolia leve (chuva, manhã quieta, sozinho). Combinação rara: *paz com sombra*. Tags: `emocao/serenidade`, `emocao/melancolia`. As duas — são polos de Plutchik (alegria↔tristeza), e podem coexistir.

**Imagem:** vai pra `Nun/_anexos/`. Nome: `luz-cozinha-cafe-2026-05-21-01.jpg`.

**Ligação simbólica:** sem totem claro. Não inventar. Deixar a cena falar.

**Densidade:** média-alta (peso atmosférico, momento contemplativo). Merece pergunta de releitura.

## Output gerado

**Nome do arquivo:** `luz-cozinha-cafe-2026-05-21.md`

**Salvo em:** `Nun/`

**Imagem salva em:** `Nun/_anexos/luz-cozinha-cafe-2026-05-21-01.jpg`

**Conteúdo da nota:**

```markdown
---
criado: 21/05/2026 às 07:18
sala: A Galeria de Hator
tags: [emocao/serenidade, emocao/melancolia, luz, cafe, chuva, manha-lenta, cozinha]
estado: semente
companhia: sozinho
lugar: cozinha de casa
humor: contemplativo
---

*21/05/2026 — 07:18*

---

# A luz da cozinha agora cedo

![[luz-cozinha-cafe-2026-05-21-01.jpg|luz dourada baixa entrando pela janela da cozinha, xícara escura sobre a bancada com vapor subindo, vidro embaçado lá fora indicando chuva fina]]

Tomei meu café aqui ouvindo a chuva começar lá fora.

A luz veio rasante, baixa, daquele dourado que só aparece nos primeiros minutos do dia — entrou pela janela e pousou na bancada antes de seguir adiante. O vapor da xícara fez um corte vertical no feixe. Lá fora, o vidro embaçando devagar marcava o ritmo da chuva chegando.

Tem cenas que pedem **silêncio** pra serem vistas. Esta era uma.

---

> Quando foi a última vez que você parou pra ver a manhã antes do dia começar?

→ [[Parou o Olhar]] · [[manhãs lentas]] (criar?) · [[A Galeria de Hator]]
```

## Resposta da skill pro Pedro

> Guardado em Nun como `luz-cozinha-cafe-2026-05-21.md`, com a foto anexa. Sugeri [[A Galeria de Hator]]. Quer ajustar?

## Notas sobre escolhas feitas

### Sobre a imagem

- **Nome do arquivo da imagem:** `luz-cozinha-cafe-2026-05-21-01.jpg` — mesmo slug da nota + sufixo `-01`. Se viessem três fotos do mesmo momento, seriam `-01`, `-02`, `-03`.
- **Pasta:** `Nun/_anexos/` — sempre. A imagem fica perto da nota, mas em subpasta dedicada pra não poluir o Nun com arquivos não-`.md`.
- **Posicionamento no .md:** logo após o H1, antes do primeiro parágrafo. A foto é entrada visual.
- **Sintaxe Obsidian:** `![[arquivo|alt text]]` — sem path, porque Obsidian resolve. O pipe (`|`) separa o nome do alt text.
- **Alt text descritivo:** "luz dourada baixa entrando pela janela da cozinha, xícara escura sobre a bancada com vapor subindo, vidro embaçado lá fora indicando chuva fina" — o que tem de essencial na imagem, em uma frase. Se a imagem quebrar daqui a 10 anos, Pedro ainda lê o que era.

### Sobre o texto

- **Título "A luz da cozinha agora cedo"** — pega o sujeito dominante (a luz) e o tempo (agora cedo). O "agora" vai virar passado quando ele reler, e isso ganha peso afetivo.
- **Primeiro parágrafo curto, quase intocado.** Pedro escreveu uma frase só sobre tomar café ouvindo a chuva. A skill manteve essa frase como abertura — sem expandir, sem decorar.
- **Segundo parágrafo é a descrição atmosférica do que a skill viu na imagem.** Não repete que Pedro tomou café (ele já disse). Complementa: a qualidade da luz (rasante, baixa, dourada de primeira hora), o detalhe do vapor cortando o feixe, o vidro embaçando como marcador de tempo. Tudo é leitura da foto — nada inventado.
- **Terceiro parágrafo é um vinco.** Uma frase só. "Tem cenas que pedem **silêncio** pra serem vistas. Esta era uma." Marca a presença sem decorar demais.
- **Negrito em "silêncio".** Uma palavra. Carrega o peso do momento.
- **Pergunta de releitura:** "Quando foi a última vez que você parou pra ver a manhã antes do dia começar?" — abre uma porta retrospectiva. Não é "como você se sentiu" (esfriaria); é uma pergunta que devolve o gesto.
- **Link `[[manhãs lentas]] (criar?)`:** indica nota-conceito potencial. Se Pedro tiver outras capturas de manhãs assim, pode virar nota-conceito reunindo todas.

### Sobre tags emocionais simultâneas

- `emocao/serenidade` + `emocao/melancolia` — duas tags emocionais em polos opostos de Plutchik (alegria leve ↔ tristeza leve). Coexistem legitimamente nesta cena. A skill não força escolher uma só. A roda das emoções autoriza simultaneidade.

### Sobre `humor: contemplativo`

- Pedro não disse "tô contemplativo". Mas o conjunto do registro (parar, observar, ouvir chuva, tomar café devagar) autoriza a skill a propor uma palavra pro humor. Se errasse, Pedro corrigia: "tava mais nostálgico". A skill propõe, não impõe — e o campo do frontmatter aceita correção fácil.

## O que esta captura faz que a anterior não fazia

- Inclui tratamento de imagem (anexo + alt text + descrição no corpo).
- Usa duas tags emocionais em polos opostos — exemplo de emoções simultâneas.
- O segundo parágrafo é leitura da imagem, não elaboração do texto. Mostra que a skill **vê** a foto, não só recebe.
- Preenche `humor:` proativamente (com palavra que parece justa pelo contexto). Mostra como o frontmatter ganha textura sem ser preenchido por Pedro a mão.

## O que esta captura NÃO faz

- Não descreve a foto de forma técnica ou exaustiva (sem "imagem em formato JPG, 4032x3024 pixels"; sem "luz dourada com temperatura de cor aproximada de 3000K"). Atmosfera, não inventário.
- Não inventa narrativa que Pedro não deu. Ele não disse que estava feliz, nem triste, nem solitário em sentido carregado. A skill respeita o silêncio dele e marca só o que está visível.
- Não usa H2 ou H3. A nota é curta, prosa primeiro.
- Não cria pasta nem nada — só consulta `Nun/` e `Nun/_anexos/` (que já existem; se não existissem, a skill criaria silenciosamente).
