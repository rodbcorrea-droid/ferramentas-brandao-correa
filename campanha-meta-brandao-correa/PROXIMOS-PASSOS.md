# Próximos passos (retomada em sessão nova)

**Estado em 2026-10-24.** Foi criada só a campanha, pausada e sem gasto. Conjuntos e anúncios **não existem**. Eles falharam duas vezes com o mesmo erro: a conexão do Meta Ads não tem a permissão `pages_manage_ads` para a Página, então não consegue ler nem usar o aceite dos termos de lead ads.

## 1. Destravar (só você pode fazer)

1. Abra https://claude.ai/customize/connectors e **reconecte o Meta Ads**, concedendo `pages_manage_ads` à Página “Brandão Correa Assessoria Jurídica” (`2033836416865143`). Seu usuário precisa ter papel de **administrador** nessa Página.
2. **Inicie uma sessão nova.** Os conectores só são lidos quando a sessão começa; reconectar não afeta uma sessão em andamento.
3. Suba os 15 arquivos de `materiais-finais/criativos-corrigidos/` na **biblioteca de mídia** da conta `1155384176705579`.

## 2. Texto para colar na sessão nova

> Leia `campanha-meta-brandao-correa/PROXIMOS-PASSOS.md` e `pendencias-a-confirmar.md` na branch `claude/mcp-meta-ads-analysis-d488zv`. Crie os dois conjuntos de anúncios na campanha 120248155947710591 e depois os anúncios com as imagens da biblioteca de mídia. Não ative nada sem eu confirmar.

## 3. Dados para criar os conjuntos (já decididos)

| Item | Valor |
|---|---|
| Conta | `1155384176705579` |
| Campanha | `120248155947710591` (pausada; objetivo Leads; **nenhuma categoria especial declarada**, sem orçamento na campanha) |
| Página | `2033836416865143` |
| Formulário | `1969971681038634` |
| Otimização | `LEAD_GENERATION`, destino `ON_AD`, cobrança `IMPRESSIONS` |
| Público | Brasil inteiro (decisão A), pessoas que moram no local, **homens, 22 a 65+**, Advantage+ Audience ligado |
| Conjunto 1 | `SUDESTE \| HOMENS \| 22+ \| AMPLO ADVANTAGE+ [RESTRINGIR ESTADOS ANTES DE ATIVAR]`, R$ 30/dia (`daily_budget` 3000) |
| Conjunto 2 | `SUL+CENTRO-OESTE \| HOMENS \| 22+ \| AMPLO ADVANTAGE+ [RESTRINGIR ESTADOS ANTES DE ATIVAR]`, R$ 20/dia (`daily_budget` 2000) |

**Atenção sobre gênero.** Com Advantage+ Audience ligado, “homens” e a idade máxima são **sugestões** para a Meta, não limites rígidos. Para forçar apenas homens, o Advantage+ Audience precisa ser desligado, o que o cliente ainda não pediu. Decidir com o cliente.

**Regra do cliente:** depois de criados, **ele restringe os estados no Gerenciador antes de ativar**: Sudeste = SP, RJ, MG, ES; Sul + Centro-Oeste = PR, SC, RS, MT, MS, GO, DF. Até lá, ambos alcançam o país todo.

## 4. Anúncios planejados

| Peça | Arquivos | Copy (ver `copies/`) | Nome do anúncio |
|---|---|---|---|
| A | `pa_juros-acima-da-media_…` | P05 | `ESTÁTICO \| TAXA MÉDIA \| PERGUNTA \| V04` |
| B | `pb_financiamento-quando-revistos_…` | P02 | `ESTÁTICO \| TAXA MÉDIA \| EDUCATIVO \| V04` |
| C | `pc_o-que-observar_…` | P09 | `ESTÁTICO \| CHECKLIST \| EDUCATIVO \| V04` |
| D | `pd_financiamento-quitado_…` | Q01 | `ESTÁTICO \| QUITADO \| PERGUNTA \| V04` |
| E | `pe_taxa-e-media_…` | E03 | `ESTÁTICO \| TAXA MÉDIA \| EDUCATIVO \| V05` |

- Anúncio de formulário: usar `object_story_spec` com `link_data.call_to_action = {type: LEARN_MORE, value: {lead_gen_form_id: "1969971681038634"}}`. A ferramenta de criar criativo isolado não expõe esse campo.
- Usar 4:5 no Feed e 9:16 nos Stories/Reels. Verificar se a ferramenta permite personalizar a imagem por posicionamento; se não, usar 4:5 e conferir a prévia em Stories.
- Link: a landing definida pelo cliente, **somente depois de a versão corrigida ir ao ar** (`materiais-finais/landing-alteracoes.md`).
- Com R$ 50/dia, cinco anúncios em dois conjuntos pulverizam o orçamento. Considerar começar com A, B e D.

## 5. Bloqueios que continuam fora da sua ação direta

- **Landing:** a versão corrigida não foi publicada; aprovação do advogado pendente.
- **Pixel:** a conta não tem pixel de site; o evento `Lead` no envio do formulário da landing depende dele.
- **Ativação:** só com confirmação explícita do cliente.
