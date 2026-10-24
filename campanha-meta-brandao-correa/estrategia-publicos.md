# Estratégia de públicos

## 1. Alerta antes de configurar

**[Provável] Possível categoria especial de anúncio.** Se a Meta classificar a campanha como “produtos e serviços financeiros”, a segmentação por **gênero e idade** e algumas opções de localização e de detalhamento ficam restritas ou indisponíveis. Isso poderia restringir a segmentação por gênero e idade.

**Decisão do cliente (2026-10-24, após a pesquisa em `pesquisa-publico.md`): seguir a recomendação: todos os gêneros, 22 a 65+, Advantage+ Audience ligado, sem interesses. Substitui a escolha inicial de “homens, 22+”. Na configuração, se a Meta exigir categoria ou bloquear gênero e idade, usar o permitido e registrar a diferença aqui. Não contornar a restrição.**

## 2. Público inicial solicitado

| Item | Configuração |
|---|---|
| Gênero | **Todos os gêneros** (decisão de 2026-10-24; antes: homens). Alternativa, se o cliente quiser forçar homens: desligar o Advantage+ Audience e aceitar o menor alcance. |
| Idade | 22 a 65+ |
| Localização | **Pessoas que moram nesta localização**. Evitar “estiveram recentemente” e segmentações de viagem. |
| Perfil | Quem financiou carro ou moto; contratos em andamento e quitados; interesse em veículos, financiamento, crédito, bancos, educação financeira e defesa do consumidor. |

**Medição:** depois de 10 a 14 dias, olhar o recorte por gênero e idade como leitura descritiva, comparando leads **qualificados** no Bitrix24. Moto tem viés masculino (69% dos motociclistas); criativos separados por veículo ficam para depois.

## 3. Regiões e conjuntos

| # | Conjunto | Estados | Fase 1 (R$/dia) |
|---|---|---|---|
| 1 | SUDESTE | SP, RJ, MG, ES | 30 |
| 2 | SUL | PR, SC, RS | 10 (unificado com o 3) |
| 3 | CENTRO-OESTE | MT, MS, GO, DF | 10 (unificado com o 2) |
| 4 | BRASIL ou NORTE-NORDESTE | ver abaixo | não ativar na fase 1 |

**Por que não criar os quatro conjuntos de início.** Com R$ 50/dia no total, quatro conjuntos dividem o orçamento em fatias pequenas. Cada conjunto precisa de volume para a entrega se estabilizar (referência da Meta: cerca de 50 resultados por conjunto na fase de aprendizado — **a confirmar**). Conjuntos com pouco orçamento ficam mais tempo em aprendizado e dão leitura frágil.

**Fase 1 recomendada**

- Conjunto 1 — Sudeste: R$ 30/dia.
- Conjunto único “Sul + Centro-Oeste”: R$ 20/dia.
- Comparar Sul e Centro-Oeste pelo breakdown por região, sabendo que isso é leitura descritiva, não teste causal.

**Fase 2** (orçamento maior ou volume suficiente): separar Sul e Centro-Oeste.
**Fase 3**: ativar o conjunto 4.

### Conjunto 4 — como evitar sobreposição

| Opção | Configuração | Observação |
|---|---|---|
| A (recomendada) | Norte-Nordeste: AC, AP, AM, PA, RO, RR, TO, AL, BA, CE, MA, PB, PE, PI, RN, SE | Sem sobreposição com os conjuntos 1 a 3. |
| B | Brasil, **excluindo** os estados dos conjuntos 1 a 3 | Equivale à opção A na prática. |
| C | Brasil sem exclusões | Gera sobreposição e competição entre os próprios conjuntos no leilão. Não recomendada. |

## 4. Duas possibilidades de segmentação

Não tornar todos os interesses obrigatórios ao mesmo tempo.

### A. Público amplo com Advantage+

Somente localização, idade e gênero. A Meta encontra as pessoas com maior probabilidade de resposta. Menor risco de restringir demais o público.

### B. Público com sugestões de interesses

Sugestões, se existirem na conta (**não usar IDs inventados**; buscar na ferramenta de interesses):

- Financiamento de veículos; Financiamento; Crédito; Bancos; Serviços financeiros;
- Carros; Automóveis; Motocicletas; Compra de automóveis; Financiamento de automóveis; Compra de motocicletas;
- Educação financeira; Defesa do consumidor; Direitos do consumidor.

**Registrar na campanha:** com Advantage+, a Meta pode expandir a entrega para além dos interesses definidos quando considerar que isso melhora o desempenho. Interesses e demais características viram **sugestões**, não limites rígidos. Localização e exclusões continuam como controles.

## 5. O que nunca usar na segmentação ou no texto

Nada que sugira que o anunciante sabe que a pessoa:

- está endividada ou inadimplente;
- foi enganada ou pagou juros abusivos;
- está em dificuldade financeira;
- tem um contrato específico;
- está em processo judicial.

Não criar segmentações que impliquem conhecimento de situação financeira vulnerável.

## 6. Remarketing

### Públicos (a criar manualmente)

| Público | Fonte (Central de Contas) | Observação |
|---|---|---|
| Assistiu a 25% do vídeo | Visualizações de vídeo | Topo do funil de remarketing |
| Assistiu a 50% do vídeo | Visualizações de vídeo | Mais engajado |
| Interagiu com o Instagram | Perfil comercial | Requer vínculo da conta (a confirmar) |
| Interagiu com a Página do Facebook | Página | |
| Abriu o formulário, mas não enviou | Formulário instantâneo | Público de abandono |
| Enviou o formulário | Formulário instantâneo | Usado para exclusão |
| Visitantes da landing page | Pixel/evento no site | **A confirmar** se o pixel está instalado em `bitrix24.site` |
| Iniciou atendimento | Lista do CRM (Bitrix24) | Exige tratamento de dados e base legal (LGPD). A confirmar |

**Estado da conta `1155384176705579` (2026-10-24): nenhum público personalizado existe e não há pixel de site.** Portanto: os públicos de vídeo, Instagram, Página e formulário só passam a acumular **depois** que houver anúncios no ar; “visitantes da landing page” exige instalar um pixel antes. Remarketing não é utilizável no lançamento. Tamanho mínimo de público e janela de retenção dependem da conta (**a confirmar**).

### Exclusões obrigatórias

- Nos conjuntos de **prospecção**: excluir quem enviou o formulário e quem iniciou atendimento.
- Nos conjuntos de **remarketing**: excluir quem enviou o formulário e quem iniciou atendimento.
- Revisar as exclusões a cada quinzena.

### Cuidados de texto

Não revelar que a plataforma sabe que a pessoa viu o vídeo, visitou a página, abriu ou abandonou o formulário ou interagiu com o anúncio. Usar as copies de `copies/copies-remarketing.md`. Não usar: “Sabemos que você viu nosso anúncio”, “Você abandonou o formulário”, “Estamos acompanhando você”, “Você visitou nossa página”.

## 7. Resumo das fases

| Fase | Quando | Conjuntos ativos |
|---|---|---|
| 1 | Lançamento | Sudeste (R$ 30) + Sul/Centro-Oeste unificado (R$ 20) |
| 2 | Volume ou orçamento maiores | Sudeste, Sul e Centro-Oeste separados |
| 3 | Após leitura consistente | Adicionar conjunto 4 e teste com todos os gêneros (com autorização) |
