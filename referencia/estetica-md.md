# Estética do .md — princípios de formatação

Este arquivo orienta a forma das notas que a skill produz. Não é manual de Markdown técnico. É o jeito como uma nota fica bonita de abrir, fácil de ler, e coesa com as outras — pra o vault inteiro respirar a mesma língua visual.

A beleza aqui não é ornamento. É método. Nota bonita convida retorno; retorno mantém memória viva. O Per Ankh inteiro depende desse princípio.

## O contexto importa

As notas desta skill **não são README de projeto**. Não são documentação técnica. Não são post de blog. São entradas de **diário simbólico** num vault pessoal.

Isso muda tudo:

- Sem badges, sem status icons, sem índice clicável, sem TOC.
- Sem blocos de código (a não ser que Pedro literalmente registre código).
- Sem tabela complexa (a não ser que faça sentido — captura de uma comparação que ele fez).
- Sem checklist técnico, sem sintaxe de issue tracking.

A referência aqui é mais próxima de **livro de visitas íntimo + catálogo de museu pessoal**.

## Os cinco princípios

### 1. Hierarquia visual clara, mas discreta

- **H1** — título da nota. Frase poética, não etiqueta. Aparece uma vez por nota, no topo. Exemplo: `# O pássaro no parque hoje` — não `# passaro_parque_2026`.
- **H2** — usar só quando a nota se divide em momentos distintos que merecem ser separados (raro em captura simples; comum no modo Scriptorium quando a nota cresceu). Exemplo: `## O que vi` / `## O que ficou` / `## Pra onde isso aponta`.
- **H3** — usar quase nunca em capturas. Reservado pra notas-conceito ou MOCs do Universo de Memórias.

A regra é: **prosa primeiro, estrutura depois**. Estrutura é convidada, não anfitriã.

### 2. Ritmo — a tipografia invisível

O Markdown não tem fonte global, então o "design" emerge do **ritmo** que a formatação cria.

- **Parágrafos curtos.** Duas a quatro frases, no máximo. Quebrar quando o pensamento muda de direção.
- **Negrito sutil.** Uma palavra por nota, no máximo duas. Pra o olho ter onde pousar. Negrito demais perde o efeito.
- **Itálico** no timestamp e em frases de meta-observação (`*Talvez também more em [[X]].*`).
- **Linha horizontal** (`---`) como pausa visual. Usar entre o timestamp e o título, e antes da pergunta de releitura. Pausa, não decoração.
- **Espaço em branco** entre parágrafos. Sempre uma linha vazia. Densidade visual cansa.

### 3. Imagens com cuidado

- **Alt text descritivo sempre.** `![[arquivo|passaro branco andando na grama molhada]]` — nunca só `![[arquivo]]`. O alt text é o que aparece se a imagem quebrar e é o que cega-de-imagem (literal ou metafórica, ao reler dali a anos) lê.
- **Posicionamento:** logo após o H1, antes do primeiro parágrafo. A imagem é entrada visual, não interrupção do texto.
- **Tamanho:** Obsidian renderiza no tamanho original. Não usar redimensionamento (`![[arquivo|300]]`) a menos que a imagem seja literal-grande demais.
- **Galeria de múltiplas imagens** (mesma cena): uma após a outra, sem texto entre elas. O texto vem depois.

### 4. Coerência — todas as notas falam a mesma língua

A skill produz centenas de notas ao longo do tempo. Se cada uma tiver uma estética própria, o vault vira colcha de retalhos. Se todas seguem a mesma gramática, o vault vira biblioteca.

**Decisões fixas da gramática:**

- Sempre frontmatter com os mesmos campos (na mesma ordem).
- Sempre timestamp em itálico antes do título.
- Sempre H1 com frase poética.
- Sempre links no fim com seta `→`.
- Sempre tags emocionais com namespace `emocao/nome`.
- Sempre alt text em imagem.
- Sempre data no nome do arquivo (`-YYYY-MM-DD`).

**Decisões variáveis (caso a caso):**

- Quantos parágrafos.
- Se tem H2.
- Se tem ligação simbólica.
- Se tem pergunta de releitura.
- Quantas tags.

Coerência no que estrutura; liberdade no que respira.

### 5. Usabilidade interna

O .md é bonito quando se mostra fácil de **reler dali a meses**:

- O título conta o suficiente pra Pedro lembrar do que era.
- O primeiro parágrafo dá o registro bruto, pra ele revisitar o momento.
- A linha horizontal separa o que era dele do que veio depois (elaboração, ligação, pergunta).
- Os links no fim convidam navegação sem cobrar.
- O frontmatter responde sem ser lido em prosa: que dia, que sala, que emoção, com quem, onde.

Pedro pode entrar numa nota antiga e em 5 segundos saber se ela merece visita longa ou cumprimento rápido.

## O que evitar

- **Excesso de emojis no corpo.** Os ícones das salas já existem no nome delas (𓁹, ☥, 𓀀, etc). Emoji em prosa só se tiver função simbólica clara. Evitar emoji decorativo (☀️ no fim de parágrafo, 💔 pra marcar tristeza, etc).
- **Headers só pra organizar pensamento que não pediu organização.** Se a captura é "vi uma íbis", não precisa de H2 "O que aconteceu" / H2 "Reflexão".
- **Listas de bullet por hábito.** Listas só quando a coisa é genuinamente lista (vários itens paralelos). Prosa antes.
- **Negrito em frases inteiras.** Negrito é pontual. Frase inteira em negrito perde peso.
- **Linhas horizontais demais.** Duas por nota é o máximo (uma após timestamp, uma antes da pergunta de releitura).
- **Citação (`>`) usada como bloco decorativo.** Usar callout `> [pergunta de releitura]` é o uso legítimo. Não usar `>` só pra dar destaque visual.
- **Frontmatter com campos inventados na hora.** Os campos são fixos: `criado`, `sala`, `tags`, `estado`, `companhia`, `lugar`, `humor`. Acrescentar campo novo só em conversa com Pedro.

## Inspirações estéticas

O ideal estético da skill bebe de:

- **Catálogos de museu** — descrição precisa, hierarquia clara, espaço em branco generoso.
- **Diários ilustrados antigos** — texto + imagem em diálogo, sem decoração entre eles.
- **Notas de Caderno de Campo de naturalista** — observação primeiro, interpretação depois, perguntas no fim.
- **Cartas pessoais** — voz íntima, ritmo de quem fala com quem conhece.

## Quando a captura é cru demais

Tem momentos em que Pedro só vai mandar uma frase curtíssima ou uma palavra solta ("vi"). A skill ainda precisa produzir nota coesa.

Nesses casos:

- O H1 vira frase curta mas presente ("Vi algo, hoje").
- A prosa pode ser uma frase só, em itálico, marcando a brevidade do gesto.
- O frontmatter fica mais vazio que o normal — campos opcionais ficam em branco.
- A pergunta de releitura não aparece (a captura não tem densidade pra pedir).
- Os links no fim aparecem mas só com a sala e talvez o guardião.

A nota fica curta. Tudo bem. A consistência da gramática mantém ela parte da casa.

## Lembrete final

A estética serve à **memória**, não à exibição. Nota bonita é a que Pedro vai abrir dali a um ano e vai sentir que ainda é dele. Toda decisão visual passa por essa pergunta:

> Isso ajuda Pedro a reler com presença, ou só está aqui pra parecer bonito?

Se a resposta é "só pra parecer bonito", cortar.
