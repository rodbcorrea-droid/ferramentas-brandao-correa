# Revisão dos materiais prontos do cliente

**Data:** 2026-10-24 · **Critérios:** `frases-proibidas-e-substituicoes.md`, `checklist-meta.md`, `checklist-publicidade-juridica.md`, `../criativos/especificacoes-estaticos.md` e o briefing.

**Veredito resumido**

| Material | Veredito |
|---|---|
| Landing page (`landing-revisao-veiculos.html`) | **Reprovada.** 3 problemas bloqueantes que contradizem o briefing e os próprios anúncios. |
| Criativo B (4:5, “Financiamento de carro ou moto”) | **Quase pronto.** Correções menores. |
| Criativo A (9:16, “Juros acima da média…”) | **Aprovável após reposicionar elementos.** |
| Criativos C e D (“O que observar…” e “Já quitou…”) | **Não publicar como estão.** Sem aviso jurídico. |
| Criativo E/F (1:1 e 9:16, “Financiou carro ou moto? Você sabe se a taxa do seu contrato está acima da média?”) | **Não publicar como está.** Sem aviso jurídico, pergunta direta sobre o contrato da pessoa e barras que sugerem taxa acima da média. |

O mais importante: **os criativos são mais cautelosos que a landing page.** O criativo A diz que juros acima da média **não** são sempre abusivos. A landing diz que a pessoa “pode ter pago juros abusivos sem saber” e que o entendimento dos tribunais é “pacificado”. Um anúncio sóbrio levando a uma página promocional é o cenário em que a página reprova e arrasta a conta.

## 1. O que foi revisado e o que não foi

| Recebido | Observação |
|---|---|
| 1ª remessa: 5 imagens | **4 distintas** (duas idênticas byte a byte) |
| 2ª remessa: 5 imagens | **2 novas salvas** (E 1:1 e F 9:16). Um “Já quitou” 1:1 também chegou, mas só foi visto na conversa; **não foi salvo em disco**. O restante repete a 1ª remessa. |
| `landing-revisao-veiculos.html` (2 envios) | Lido por inteiro. **Os dois envios têm o mesmo checksum (conteúdo idêntico): nenhum item foi corrigido entre eles.** **Assumo que é o conteúdo publicado em `https://acidentesinss.bitrix24.site/jurosfinan/`**; a URL ao vivo não pôde ser aberta pelo ambiente. |

| Não recebido / não revisado | Por quê |
|---|---|
| Versões 1:1 de A, B e C; 4:5 de A, C, D e E; 9:16 de B | Não chegaram. O pacote exige 1:1, 4:5 e 9:16. |
| Criativo “**escondidas**” (`criativo3_escondidas`) | Nenhuma imagem traz esse texto. **[Palpite]** o nome é um rótulo interno da peça C (“Seguro prestamista”, “Tarifas e encargos”); não consigo confirmar a ligação entre nomes de arquivo e imagens. |
| Vídeo da landing (Vimeo `1224326477`) | O HTML só incorpora o player. |
| Formulário da landing (Bitrix24, `inline/117/ih752e`) | Carregado de um script externo; não vi campos nem texto de consentimento. |

Os arquivos estão em `../materiais-finais/`. Nomes originais dos PNGs não são conhecidos; os arquivos foram nomeados pelo conteúdo.

## 2. Landing page

Gravidade: 🔴 bloqueante · 🟠 alto · 🟡 médio · ⚪ baixo. Linhas referem-se ao HTML recebido.

| # | Gravidade | Achado (trecho exato) | Regra | Correção sugerida |
|---|---|---|---|---|
| L1 | 🔴 | H1 (linhas 439–444): “Financiou Carro ou Moto nos Últimos 10 Anos? **Você Pode Ter Pago Juros Abusivos Sem Saber.**” | Frase proibida (“Você certamente pagou juros abusivos”; “vítima de juros abusivos”) e atributos pessoais. Contradiz o criativo A. | “A taxa do financiamento pode ser analisada.” + subtítulo do briefing |
| L2 | 🔴 | **Três depoimentos** com 5 estrelas (linhas 612–657): Carlos M., Rodrigo S., Fernanda L., com desfechos (“Recálculo pela Taxa do BACEN”, “Restituição de Seguros Ocultos”, “Contrato Quitado Revisado”, “entrou com o pedido de restituição”). | Briefing: não inventar depoimentos. **[Provável]** o Provimento 205/2021 veda depoimentos e divulgação de resultados. O rodapé da própria página cita “estrita observância ao Provimento nº 205/2021”. | Remover a seção. Se os depoimentos são reais, ainda assim remover. |
| L3 | 🔴 | **Quiz** (linhas 531–587, 794–802): toda combinação de respostas, inclusive “Não tenho certeza”, termina em “**Caso Enquadrado para Análise Técnica** — Seu contrato pode ter direito à Revisão e Restituição!”. O passo 2 pergunta “Estou com parcelas em atraso no momento”. | Triagem de fachada que sugere direito a todos. Coleta, na página, situação financeira vulnerável sem finalidade nem armazenamento definidos (LGPD). | Remover o resultado fixo ou trocar por “Obrigado. A equipe fará uma análise inicial. Não há promessa de resultado.” Remover a opção de atraso. |
| L4 | 🟠 | Alegações absolutas: “entendimento **pacificado**” (596), “**Jurisprudência Consolidada**” (498), “Até 10 Anos — Prazo para Revisar” (497), “**inclusive já quitados**” (418, 447), pílula “Restituição de Venda Casada” (453), “Tema 972” (597). | Contradiz os criativos (“não automaticamente”, “dependem”). **[Provável]** a posição do STJ é que juros acima da média não são, por si só, abusivos; exige-se discrepância relevante. Conferir com o advogado. | Reescrever com “pode”, “conforme o caso”, sem “pacificado” nem “consolidada”. |
| L5 | 🟠 | Card “**Seguros e Taxas Ocultas (Venda Casada)**” (517–521): “É muito comum os bancos embutirem…”. | Acusa instituições de forma genérica (critério do briefing). | Descrever o que pode ser observado, sem imputar prática aos bancos. |
| L6 | 🟠 | **Sem link para a política de privacidade** (nenhum `<a href>` na página; “privacidade” e “política” aparecem 0 vezes). Sem aviso de cookies nem consentimento visível. | Exigência de LGPD e do formulário/landing. | Linkar `https://brandaocorrea.bitrix24.site/politica/` no rodapé e no modal. |
| L7 | 🟠 | **Rastreamento quebrado**: o código chama `fbq('trackCustom','QuizCompleted')` e `fbq('track','InitiateCheckout')`, mas **não há código-base do pixel**, e a conta não tem pixel de site. Abrir o formulário é registrado como `InitiateCheckout` (evento de compra). | Nenhum evento será medido. Evento incorreto polui a otimização. | Instalar o pixel; disparar `Lead` no envio do formulário. |
| L8 | 🟠 | **Alcance geográfico**: “Direito Bancário e Revisão Contratual **em Mato Grosso**”, “Atendimento 100% Digital — **em todo MT**”, jurisprudência do **TJMT**, “Cuiabá/MT”. A campanha mira SP, RJ, MG, ES, PR, SC, RS, MT, MS, GO, DF e Brasil. | Desalinhamento anúncio × página. **[Provável]** o Estatuto da Advocacia (art. 10, §2º) exige inscrição suplementar na seccional em que o advogado atua habitualmente (mais de cinco causas por ano). Pergunta para o advogado, antes de segmentar fora de MT. | Alinhar a página ao alcance real, ou restringir a campanha a MT. |
| L9 | 🟠 | “**Atuação especializada** em Direito Bancário e Defesa do Consumidor” (602). O site principal do cliente se apresenta como especialista em INSS. | **[Palpite]** anunciar especialização pode exigir título. | Trocar por “atuação em…”, se confirmado. |
| L10 | 🟡 | Pressão: barra superior com id `urgency-bar` e ponto pulsante, botão pulsante, **modal de saída** (“Antes de sair, lembre-se…”) que repete as alegações absolutas. “Sigilo Profissional **Garantido**” (486). | Briefing: sem urgência artificial. | Remover modal de saída e animações pulsantes; trocar “Garantido” por “Sigilo profissional”. |
| L11 | 🟡 | Vídeo com autoplay mudo e “Toque para ouvir a explicação”. | Conteúdo do vídeo não revisado. | Enviar o vídeo para revisão. |
| L12 | ⚪ | Nome da marca: **“Brandão Corrêa”** (com acento) na página; **“Brandão Correa”** nos criativos e no briefing. | Não alterar o nome da marca; precisa ser uniforme. | Definir uma grafia e usar em todas as peças. |
| L13 | ⚪ | `meta description` (linha 7) repete “O STJ e o TJMT admitem a revisão… inclusive já quitados”. | Mesma alegação do L4. | Reescrever com a copy do briefing. |

**A OAB/MT 16.113** aparece em quatro pontos da página. Este pacote não a copiou para nenhum anúncio nem a validou. Se for exibida nas artes, o advogado precisa confirmar o formato exigido.

**Nota sobre a revisão da OAB.** Você informou que a revisão está feita. Os itens L2, L4, L5 e L9 contradizem o que eu entendo do Provimento 205/2021 e o que a própria página declara no rodapé. Isto me faz duvidar de que a revisão tenha incluído esta página. É uma pergunta para o advogado, não uma conclusão minha.

## 3. Criativos

| Peça | Arquivo | Formato | Pontos fortes | Achados | Gravidade |
|---|---|---|---|---|---|
| **A** “Juros acima da média são sempre abusivos? **Não automaticamente.**” | `pa_juros-acima-da-media_9x16` (2 cópias idênticas) | 9:16, 1125×2000 | Linguagem equilibrada; “É preciso analisar o contrato e as circunstâncias”; aviso presente | Logotipo e **aviso legal na faixa inferior** coberta pela interface; primeira linha do título encosta na faixa superior; aviso pequeno e de baixo contraste; contém a palavra “abusivos” (em pergunta, com resposta negativa) | 🟠 |
| **B** “Financiamento de carro ou moto — Quando os juros podem ser revistos?” | `pb_financiamento-quando-revistos_4x5` | 4:5, 1024×1280 | Aviso legível (“Não há garantia de resultado”); texto hedged; formato correto para o Feed | Carro e moto parecem **modelos reconhecíveis** de mercado (o briefing pede imagens genéricas); logotipo diferente do das outras peças | ⚪ |
| **C** “O que observar no financiamento do seu veículo” | `pc_o-que-observar_9x16` | 9:16, 941×1672 | Estrutura em lista, tom informativo | **Sem aviso jurídico.** Moedas e “$” sobre lupa, com CTA “Conheça seus direitos”, sugerem recuperação de dinheiro. “Seguro prestamista” está **fora do escopo do briefing** e depende do respaldo da landing (L5). Título na faixa superior; logotipo e botão na inferior | 🔴 |
| **D** “Já quitou o financiamento? A revisão do contrato pode ser discutida mesmo após a quitação.” | `pd_ja-quitou_9x16` | 9:16, 941×1672 | “Prazos e cabimento dependem do histórico do contrato” modera a afirmação | **Sem aviso jurídico.** Abre com pergunta sobre atributo pessoal (“Já quitou…?”). Selo “QUITADO” e CTA “Conheça seus direitos”. Título na faixa superior; logotipo e botão na inferior | 🔴 |

**Pontos comuns**

- **Logotipo inconsistente:** três emblemas diferentes (brasão heráldico na A, brasão prateado pequeno na B, escudo com balança em C e D). O briefing proíbe criar logotipo. **Confirme que cada emblema é o oficial**; se algum foi desenhado por IA, substitua pelo arquivo oficial. **Parece** haver uma balança dentro de escudo em C e D, que pode ser lida como símbolo de decisão favorável. Conferir.
- **Zonas seguras** (referência de 250 px no topo e 340 px na base em 1080×1920, a confirmar com a Meta): o logotipo cai na faixa inferior nas três peças 9:16; o título cai na faixa superior em C e D; os botões de C e D encostam na faixa inferior.
- **Formatos incompletos:** só B está em 4:5; nenhuma peça está em 1:1; A, C e D só em 9:16.
- **CTA “Conheça seus direitos”** é permitido pelo checklist **apenas** se não prometer resultado (a confirmar com o advogado). Em C e D, junto de moedas e selo, o risco aumenta.

## 4. Ordem de correção

1. **Landing (L1, L2, L3, L5):** remover antes de qualquer envio. Sem isso, a campanha não deve subir.
2. **Landing (L6, L7):** link da política e pixel com evento `Lead`.
3. **Criativos C e D:** incluir aviso curto; reposicionar título, botão e logotipo dentro das zonas seguras.
4. **Criativo A:** subir logotipo e aviso para fora da faixa inferior; aumentar o contraste do aviso.
5. **Logotipo oficial** em todas as peças e **uma só grafia** do nome.
6. **Formatos faltantes** (1:1 de todas; 4:5 de A, C e D).
7. **Perguntas para o advogado:** L4, L8, L9 e a questão dos depoimentos (L2).
8. Landing L10 a L13 e vídeo (L11).

## 5. Atualização — segunda remessa (2026-10-24)

**Landing: idêntica à primeira.** Os dois HTML enviados têm o mesmo checksum. Se você editou a página, o arquivo enviado não é o editado. **Todos os achados L1 a L13 continuam valendo.**

**Peças novas**

| Peça | Arquivo | Formato | Achados | Gravidade |
|---|---|---|---|---|
| **E** “Financiou carro ou moto? Você sabe se a taxa do seu contrato está acima da média?” | `pe_financiou-taxa-vs-media_1x1` | 1:1, 1254×1254 | **Sem aviso jurídico.** Pergunta direta sobre o contrato da pessoa (“Você sabe… do **seu** contrato”), mesmo risco de atributos pessoais já apontado em P01/P11. Barras: a do contrato é cerca de **1,8 vez** a da média, o que sugere taxa acima da média; a ressalva “comparação ilustrativa” é minúscula. CTA “Conheça seus direitos”. | 🔴 |
| **F** (mesma arte) | `pf_financiou-taxa-vs-media_9x16` | 9:16, 940×1672 | Os mesmos achados de E. Primeira linha do título dentro da faixa superior; logotipo dentro da inferior; botão rente ao limite. | 🔴 |
| **D** “Já quitou o financiamento?” | só visto na conversa | 1:1 | Mesmos achados de D 9:16: **sem aviso**, pergunta sobre atributo pessoal, selo “QUITADO”, CTA “Conheça seus direitos”. Esta versão adiciona rótulo “CONTRATO DE FINANCIAMENTO” e uma assinatura desenhada. | 🔴 |

**Ponto forte de E/F.** A frase “**Superar a média, isoladamente, não comprova abusividade**” é honesta e está alinhada com o criativo A. É também o oposto da landing (“entendimento pacificado”, “Você pode ter pago juros abusivos”). **[Provável]** é a posição mais próxima do entendimento do STJ. Use-a como base para reescrever a landing.

**Logotipo.** Os emblemas continuam diferentes entre as peças (brasão heráldico em A, brasão prateado pequeno em B, escudo com balança em C a F). Confirme o oficial.

**Estado dos formatos recebidos**

| Peça | 1:1 | 4:5 | 9:16 |
|---|---|---|---|
| A “Juros acima da média…” | — | — | ✅ |
| B “Financiamento de carro ou moto” | — | ✅ | — |
| C “O que observar…” | — | — | ✅ |
| D “Já quitou…” | ✅ (não salvo) | — | ✅ |
| E/F “Financiou carro ou moto?” | ✅ | — | ✅ |

## 6. O que este relatório não faz

Não corrige os arquivos, não altera a landing publicada nem sobe nada ao Meta. As correções de texto acima são sugestões a serem aprovadas pelo advogado responsável.
