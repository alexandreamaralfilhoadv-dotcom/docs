---
name: pesquisa-jurisprudencial
description: "Padrão de toda pesquisa jurisprudencial feita para Alexandre: primeiro consulta a pasta Jurisprudência do Google Drive dele e só depois os sites; cada precedente vem com link direto para a fonte oficial (inteiro teor ou página do processo), dados completos de identificação e menção expressa ao peso do precedente (vinculante, repetitivo, repercussão geral, súmula ou isolado), para que ele mesmo confira antes de usar. Use SEMPRE que ele pedir pesquisa de jurisprudência, precedentes, julgados, entendimento do STF/STJ/TST/TRFs/TJs, súmulas, temas repetitivos ou de repercussão geral, 'como os tribunais decidem X', 'tem julgado sobre Y', ou pedir para fundamentar uma tese com decisões, mesmo sem dizer 'jurisprudência'. Também vale quando outra skill (peticoes, materiais-estudo, lei-comentada) precisar buscar precedentes."
---

# Pesquisa jurisprudencial: padrão de entrega

## Objetivo

Alexandre usa a pesquisa como ponto de partida, não como produto final. Ele vai abrir cada link,
ler o acórdão e conferir os dados antes de citar em peça, parecer ou material de estudo. Por isso,
toda pesquisa precisa ser **rastreável**: cada precedente vem com o caminho exato até a fonte e com
os dados necessários para localizá-lo de novo, mesmo se o link quebrar.

## Regras inegociáveis

1. **Sempre traga o link.** Todo precedente citado vem com link clicável para a fonte oficial.
   Sem link, o precedente não entra na lista principal.
2. **Nunca invente precedente, número, relator, data ou link.** Se não conseguir confirmar algum
   dado, escreva `[verificar]` no campo. Não complete por dedução.
3. **Link de busca não substitui link do julgado.** Se só houver como apontar a página de pesquisa
   do tribunal, deixe isso explícito ("link de pesquisa pré-filtrada, não do acórdão") e informe os
   termos exatos para ele refazer a busca.
4. **Separe o que foi verificado do que não foi.** Precedentes que você não conseguiu abrir ou
   confirmar vão para uma seção própria no fim, nunca misturados aos confirmados.

## Etapa 1: consultar primeiro a pasta "Jurisprudência" do Google Drive

Antes de qualquer busca na internet, consulte a pasta **Jurisprudência** do Google Drive de
Alexandre pelo conector do Google Drive.

- **Pasta:** Jurisprudência
- **ID:** `1trEsqWYrMijLKsPDWvtypunlAi7-LnTr`
- **Link:** https://drive.google.com/drive/folders/1trEsqWYrMijLKsPDWvtypunlAi7-LnTr

Como fazer:

1. Liste o conteúdo da pasta (`parentId = '1trEsqWYrMijLKsPDWvtypunlAi7-LnTr'`), incluindo
   subpastas, se houver. A pasta pode receber arquivos novos, então liste sempre; não presuma o
   conteúdo.
2. Busque o tema dentro dos arquivos com `fullText contains '<termo>'` restrito à pasta, usando
   sinônimos e o número de súmula ou tema quando souber. Abra os arquivos relevantes para ler o
   trecho exato.
3. Hoje a pasta reúne compilações de súmulas, temas repetitivos, teses vinculantes e orientações
   (STF, STJ, TST e AGU) e um material de revisão anotado. Use-as para identificar rapidamente
   súmulas, temas e teses ligados à pergunta.

Como usar o que encontrar:

- Abra a resposta com a seção **"Na sua pasta do Drive"**, listando o que foi achado: nome do
  arquivo, link do arquivo no Drive, página ou trecho, e o enunciado (súmula, tema, tese ou OJ).
- As compilações têm data de corte (o nome do arquivo indica, como "05 10"). Por isso, **confirme
  cada item no site oficial** do tribunal na etapa seguinte, para checar se continua vigente, se
  foi revisado ou cancelado, e para trazer o link oficial. O link do Drive não substitui o link
  oficial.
- Se nada relevante for encontrado, diga isso em uma linha ("Nada sobre o tema na pasta
  Jurisprudência do Drive") e siga para a internet.
- Se o conector do Google Drive não estiver disponível, avise logo no início e siga para a
  internet.

## Etapa 2: pesquisa nos sites, por ordem de prioridade das fontes

Depois do Drive, complemente e confirme na internet. Prefira sempre a fonte primária, nesta ordem:

1. Site oficial do tribunal (inteiro teor, acompanhamento processual ou página do tema/súmula).
   - STF: portal.stf.jus.br e jurisprudencia.stf.jus.br
   - STJ: processo.stj.jus.br, scon.stj.jus.br e a página de repetitivos/IAC
   - TST: jurisprudencia.tst.jus.br e consultaprocessual.tst.jus.br
   - TRFs, TRTs e TJs: portal de jurisprudência de cada tribunal
2. Diário oficial eletrônico (DJe) com a publicação do acórdão.
3. Repositórios secundários confiáveis (JusBrasil, Dizer o Direito, Conjur, Migalhas), apenas
   quando a fonte oficial não estiver acessível. Nesse caso, sinalize "fonte secundária" e, se
   possível, indique também onde está o original.

## Formato de cada precedente

Use este bloco para cada julgado:

```
### [Tribunal] — [Classe] nº [número] / [UF]
- **Peso:** [Vinculante (Súmula Vinculante / Repercussão Geral Tema X / Repetitivo Tema X / IAC / IRDR) | Súmula | Precedente qualificado | Julgado isolado | Decisão monocrática]
- **Órgão julgador:** [Plenário / Turma / Seção / Câmara]
- **Relator(a):** [nome]
- **Julgamento:** [dd/mm/aaaa] · **Publicação:** [DJe dd/mm/aaaa]
- **Tese / síntese:** [2 a 4 linhas com o que foi decidido, nas suas palavras]
- **Trecho-chave:** "[trecho curto e literal da ementa ou do voto]"
- **Relevância para a pergunta:** [1 a 2 linhas ligando o julgado ao caso dele]
- **Link:** [URL direta para o inteiro teor ou para a página do processo]
- **Situação:** [Vigente | Superado | Em revisão | Tema com julgamento pendente] — [verificado em dd/mm/aaaa]
```

Notas sobre os campos:

- **Peso** é obrigatório e vem logo no topo. É a primeira coisa que ele precisa saber para decidir
  se o julgado sustenta a tese sozinho ou só reforça.
- **Trecho-chave** deve ser curto e literal. Nunca transcreva a ementa inteira.
- **Situação** indica se o entendimento ainda vale. Se houver overruling, distinguishing relevante
  ou tema afetado pendente, diga isso.

## Estrutura da resposta

1. **Resposta direta** (2 a 5 linhas): qual é o entendimento predominante hoje, em qual tribunal,
   e se há divergência.
2. **Na sua pasta do Drive**: o que foi achado na pasta Jurisprudência (arquivo, link, trecho) e
   se cada item foi confirmado como vigente no site oficial. Se nada foi achado, uma linha dizendo
   isso.
3. **Precedentes vinculantes e qualificados** (súmulas vinculantes, repercussão geral, repetitivos,
   IAC, IRDR, súmulas), do mais forte para o mais fraco.
4. **Julgados relevantes** (turmas, seções, tribunais locais), do mais recente para o mais antigo.
5. **Divergências ou mudanças de entendimento**, se houver.
6. **Não verificados**: precedentes mencionados em fontes secundárias que você não conseguiu
   confirmar, com o motivo e o link onde apareceram.
7. **Como refazer a busca**: termos exatos usados, filtros aplicados e links das páginas de
   pesquisa de cada tribunal consultado, para ele aprofundar por conta própria.

## Checklist antes de entregar

- [ ] A pasta Jurisprudência do Drive foi consultada antes da internet, e o resultado aparece na
      seção "Na sua pasta do Drive".
- [ ] Cada item vindo do Drive foi confirmado no site oficial ou marcado como `[verificar]`.
- [ ] Todo precedente da lista principal tem link clicável.
- [ ] Todo precedente tem o campo **Peso** preenchido.
- [ ] Nenhum dado foi completado por suposição; o que faltou está como `[verificar]`.
- [ ] Fontes secundárias estão sinalizadas como tal.
- [ ] Os não verificados estão separados no fim.
- [ ] A seção "Como refazer a busca" traz os termos e os links de pesquisa.
