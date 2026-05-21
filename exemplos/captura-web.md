# Exemplo de captura — conteúdo web

Este exemplo mostra como a skill processa uma captura que vem de leitura mediada por conteúdo externo (artigo, post, vídeo, ensaio, página) — não experiência vivida diretamente.

A pergunta central, antes de tudo: **qual é o tipo de relação do Pedro com o que ele leu?** Não é automático que conteúdo web vire "análise" ou "ideia". A skill precisa identificar:

- **Foi insight** (a leitura disparou pensamento próprio que ganhou vida fora dela) → **Alexandria**.
- **Foi análise** (Pedro está decompondo a estrutura/decisões da obra alheia) → **Mesa de Ganesha**.
- **Foi gosto / atravessamento estético** ("amei essa frase", "me prendeu") → **Câmara das Vozes**.
- **Foi reação emocional direta** (afeto bruto ao ler, antes do pensamento) → **Sala dos Afetos**.
- **Disparou criação própria** (Pedro já começou a imaginar algo dele a partir disso) → **Mesa de Toth**.
- **Reconhecimento sobre si** (a leitura virou espelho de padrão pessoal) → **Espelho de Maat**.
- **Fez pensar em pessoa** específica → **Pomar de Osíris**.

A regra de ouro: **o objeto da nota é o que vai pra sala, não o conteúdo lido em si**. O objeto pode ser a ideia que veio na cabeça do Pedro (Alexandria), a leitura crítica da obra (Ganesha), o gosto pela obra (Vozes), ou tudo ao mesmo tempo — caso em que a skill marca o foco principal e as outras como secundárias.

---

## Input do Pedro

> "li agora esse texto sobre rituais de luto no Egito antigo. tem um trecho que diz que os mortos eram visitados e *alimentados* nos túmulos, anos depois — não era homenagem só, era manutenção do vínculo. fiquei pensando se a gente perdeu isso. e me veio na cabeça uma cena pra um curta — uma mulher levando café pro pai três anos depois."

Junto, ele cola o link: `https://example.com/rituais-de-luto-egito-antigo`

A skill recebe o texto + o link.

## Leitura da skill

**Três camadas presentes na mesma captura:**

1. **Insight** (Alexandria): "a gente perdeu isso" — Pedro está pensando o presente a partir da leitura. Ideia que ganha vida fora do artigo.
2. **Atravessamento estético / gosto pelo trecho** (Vozes): o detalhe do *alimentar* o morto pegou o Pedro. Há prazer estético no detalhe.
3. **Criação própria disparada** (Toth): "me veio na cabeça uma cena pra um curta" — Pedro já está imaginando obra dele. Isso é Toth, não Ganesha (porque é criação dele, não análise da obra alheia).

**Decisão de foco:** o gesto mais carregado da captura é a **criação própria disparada**. Pedro registrou o insight rapidamente, mas o tempo que ele dedicou à cena imaginada é o que indica peso. Sala principal: **A Mesa de Toth**.

**Sala secundária:** Alexandria (o insight sobre vínculo com mortos pode virar nota-conceito autônoma; merece ligação).

**Sala terciária possível:** Pomar de Osíris (ancestralidade, mortos como presença). Marcar no corpo se fizer sentido.

**O que a skill NÃO faz:** não vai pra Ganesha. Pedro não está analisando o ensaio (estrutura, argumento, retórica do autor). Ele está usando o ensaio como matéria-prima pra pensamento e criação próprios. Ganesha exigiria análise da obra alheia em si.

**Frontmatter ganha campo `fonte:`** com o URL.

## Output gerado

**Nome do arquivo:** `rituais-luto-cena-curta-2026-05-22.md`

**Salvo em:** `Nun/`

**Conteúdo da nota:**

```markdown
---
criado: 22/05/2026 às 21:34
sala: A Mesa de Toth
tags: [emocao/sentimentalismo, luto, ancestralidade, ritual, cena, curta, egito]
estado: semente
companhia: sozinho
lugar: 
humor: pensativo
fonte: https://example.com/rituais-de-luto-egito-antigo
---

*22/05/2026 — 21:34*

---

# Uma mulher levando café pro pai três anos depois

> Li agora esse texto sobre rituais de luto no Egito antigo. Tem um trecho que diz que os mortos eram visitados e *alimentados* nos túmulos, anos depois — não era homenagem só, era manutenção do vínculo.

A frase que abriu foi "alimentados". Não visitados, não lembrados — **alimentados**. O verbo carrega obrigação de presença que a homenagem moderna perdeu.

Fiquei pensando se a gente perdeu isso mesmo, ou só perdeu a forma. Talvez o vínculo migrou pra outros gestos (foto na geladeira, prato favorito no domingo) — mas perdeu a continuidade ritualizada.

E me veio uma cena: uma mulher levando café pro pai três anos depois. Sem ironia, sem fantasia — só o gesto. Ela senta na pedra, abre a garrafa, serve dois copos, bebe o dela. Câmera fixa, tempo real. O pai não aparece. O café esfria.

*Isso é matéria pra Toth — uma cena pedindo desenvolvimento. Mas o insight sobre vínculo com mortos pode virar nota-conceito autônoma em [[A Biblioteca de Alexandria]].*

---

> Se essa cena virar curta, o que precisa estar visível pra que o gesto não vire melodrama?

→ [[Obras em Curso]] · [[manutenção do vínculo]] (criar?) · [[A Mesa de Toth]] · [[A Biblioteca de Alexandria]]
```

## Resposta da skill pro Pedro

> Guardado em Nun como `rituais-luto-cena-curta-2026-05-22.md`. Foco em Toth (a cena que apareceu); marquei Alexandria como segunda casa pra o insight sobre vínculo. Quer ajustar?

## Notas sobre escolhas feitas

### Sobre o foco em Toth, não Alexandria

- A captura tem três camadas (insight, gosto pelo trecho, cena imaginada), e qualquer uma delas poderia virar sala principal. A skill escolheu Toth porque:
  - A cena tem **detalhes concretos** (café, três anos, garrafa, dois copos, câmera fixa) — isso é matéria de criação, não pensamento abstrato.
  - O tempo que Pedro dedicou à cena no texto original é maior que o tempo dedicado ao insight. Densidade indica foco.
  - Toth abriga obras em curso; a cena claramente é uma.
- O insight sobre vínculo com mortos é marcado no corpo como **alternativa legítima pra Alexandria**, com link explícito. Pedro pode mover ou ligar no Scriptorium.

### Sobre NÃO ir pra Ganesha

- Ganesha analisa obra alheia: decompõe estrutura, decisões narrativas, retórica do autor. Pedro não fez isso. Ele usou o ensaio como gatilho, não como objeto de análise.
- Esse é o tipo de erro que a skill precisa evitar: tudo que vem da web não é Ganesha por padrão. Ganesha só quando Pedro está explicitamente lendo a obra como crítico.

### Sobre o campo `fonte:` no frontmatter

- Campo novo (opcional, só pra capturas web). URL completo. Permite Pedro reabrir a fonte se quiser revisitar o trecho original.
- Quando a fonte é citação de livro físico, o campo pode receber: `fonte: Saramago, "Memorial do Convento", p. 47`. Quando é vídeo: URL do YouTube/Vimeo com timestamp se Pedro deu.

### Sobre a citação em bloco

- O parágrafo original de Pedro vira citação em `>`, como no áudio. Separa a voz dele (registro bruto) da voz da skill (elaboração). Pedro lê e vê de longe quem disse o quê.

### Sobre o negrito em "alimentados"

- Uma palavra. Carrega o vinco do que pegou Pedro. Repete o destaque que ele mesmo deu (com itálico em "alimentados" no texto original) — mas em negrito, conforme a gramática da casa.

### Sobre a cena descrita em detalhe

- A skill **expandiu** a cena que Pedro mencionou em meia linha. Por quê? Porque Pedro estava registrando matéria de criação — não desabafo, não insight puro. Em modo Toth, a elaboração ajuda a fixar a imagem mental enquanto ela ainda é nítida. Mas o limite é claro: a skill **não inventou** elementos que Pedro não disse (sem música de fundo, sem flashback, sem segundo personagem). Só desdobrou o gesto que ele já marcou.

### Sobre a pergunta de releitura

- "Se essa cena virar curta, o que precisa estar visível pra que o gesto não vire melodrama?" — pergunta operacional pra criação, não emocional. Toth pede esse tipo de provocação. Em Hator ou Afetos, a pergunta seria outra.

### Sobre `humor: pensativo`

- Pedro não disse o humor, mas o texto inteiro carrega quietude reflexiva. A skill propõe "pensativo"; Pedro corrige se não bater.

## Variações do mesmo tipo de captura

A regra "qual é a relação?" vale também pra:

- **Artigo lido + ideia disparada** → Alexandria, com `fonte:` no frontmatter.
- **Artigo lido + análise crítica do que o autor disse** → Ganesha (raro, mas legítimo quando Pedro está estudando retórica/argumentação).
- **Crítica de filme/série + reação de gosto** → Vozes.
- **Crítica de filme/série + análise estrutural** → Ganesha.
- **Post / thread que disparou reconhecimento sobre si** → Maat.
- **Texto sobre alguém específico (artista, escritor, pensador)** → Pomar (se Pedro tem vínculo) ou Vozes (se é gosto pela figura).
- **Conteúdo que disparou criação imediata** → Toth, sempre.
- **Vídeo de YouTube** → mesma lógica; campo `fonte:` recebe URL com timestamp se ajudar a localizar o momento.

## Quando a captura web combina sala com gesto

| Pedro está fazendo | Sala |
|---|---|
| pensando o mundo a partir do conteúdo | Alexandria |
| decompondo a obra como crítico | Ganesha |
| sentindo gosto/repulsa pela obra ou trecho | Vozes |
| reagindo emocionalmente, ainda sem nomear | Afetos |
| imaginando obra própria a partir disso | Toth |
| reconhecendo padrão sobre si | Maat |
| pensando em pessoa específica | Pomar |
| atravessado por beleza (paisagem, foto, frase visual) | Hator |

## O que esta captura faz que as anteriores não faziam

- Introduz o campo `fonte:` no frontmatter (URL).
- Trabalha com três camadas simultâneas (insight + gosto + criação) e escolhe foco com critério.
- Demonstra a distinção fina Alexandria/Ganesha/Toth/Vozes.
- Mostra a skill desdobrando matéria de criação sem inventar elementos não-ditos.

## O que esta captura NÃO faz

- Não vai automaticamente pra Ganesha só porque é texto da web.
- Não analisa o ensaio em si (não comenta o argumento do autor, não avalia a tese).
- Não cita o conteúdo do link além do que Pedro já trouxe na mensagem.
- Não força a cena a ser melhor que o gesto que Pedro deu — respeita o esboço.
