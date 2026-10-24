# Pendências e informações a confirmar

Tudo o que não foi fornecido ou que depende de política vigente está listado aqui. Nada foi inventado.

Legenda: ✅ decidido/fornecido pelo cliente · ⏳ aberto · ⚠️ decidido, mas com conferência necessária · 🚫 bloqueia a criação.

## Bloqueantes (atualizado em 2026-10-24, após leitura da conta)

| # | Pendência | Estado | Nota |
|---|---|---|---|
| 1 | Categoria especial de anúncio e público “homens, 22+” | ✅ Decidido | Cliente decidiu prosseguir. Se a Meta bloquear gênero ou idade, usar o permitido, registrar e avisar. Não contornar. **Ao criar a campanha, a declaração de categoria especial é escolha do anunciante e não pode ser desfeita depois de criada**; confirmar a escolha antes de criar. |
| 2 | Regras de publicidade da OAB | ✅ Revisado pelo cliente | Este pacote não verificou a revisão. |
| 3 | Landing page | ⚠️ URL informada, conteúdo **não verificado** | `https://acidentesinss.bitrix24.site/jurosfinan/`. O ambiente do pacote não abre `bitrix24.site`. **Domínio `acidentesinss` difere do `inssacidentes` usado no repositório: confirmar a URL.** |
| 4 | Política de privacidade | ⚠️ URL informada, conteúdo **não verificado** | `https://brandaocorrea.bitrix24.site/politica/`. Conferir que abre e cobre esta finalidade. |
| 5 | Conta, Página e Instagram | ✅ Definidos | Conta `1155384176705579`; Página `2033836416865143`; Instagram `@brandaocorrea.adv` (`17841407573996167`). |
| 5a | **Termos de lead ads da Página** | 🚫 **Não aceitos (segundo a API)** | Aceitar em https://www.facebook.com/legal/leadgen/tos. Sem isso o conjunto de anúncios de leads não é criado. Se já foi aceito por outro usuário, confirmar no Gerenciador de Anúncios. |
| 5b | **Pixel no site** | ⏳ Inexistente na conta | Só há dataset de WhatsApp. Instalar um pixel na landing page se quiser *Landing page views*, remarketing por visita e eventos de site. |
| 5c | Criativos e landing prontos do cliente | ⚠️ Recebidos e **revisados** | 4 criativos distintos e o HTML da landing, em `materiais-finais/`. **Landing reprovada; criativos C e D sem aviso jurídico.** Ver `conformidade/revisao-materiais-2026-10-24.md`. 2ª remessa: landing **idêntica** (nada corrigido) e peças E/F novas, também sem aviso. Faltam 1:1 de A, B e C; 4:5 de A, C, D e E. |

## Criação no Meta (2026-10-24)

| # | Item | Estado |
|---|---|---|
| M1 | Campanha `LEADS \| Financiamento Veículos \| Análise Contratual \| BR` | ✅ **Criada, pausada, gasto zero.** ID `120248155947710591`. **É uma campanha real, não um rascunho** (o modo rascunho não está liberado nesta conta). Objetivo Leads; orçamento no nível dos conjuntos (R$ 30 + R$ 20); **nenhuma categoria especial declarada, o que não pode ser alterado depois**. Se a decisão mudar, criar nova campanha; esta está vazia |
| M2 | Conjuntos de anúncios (Sudeste; Sul + Centro-Oeste) | 🚫 **Tentativa de criação falhou** (2026-10-24). O erro informa que a Página não aceitou os termos **ou que a conexão não consegue ler o aceite**, e que isso exige a permissão `pages_manage_ads` para a Página e papel de administrador. O cliente mostrou o aceite na tela. **Ação:** reconectar o conector do Meta Ads concedendo `pages_manage_ads` à Página `2033836416865143`. Decisão do cliente: **opção A** (Brasil inteiro; restringir os estados no Gerenciador antes de ativar) |
| M3 | Formulário nativo | ✅ Criado pelo cliente. ID `1969971681038634` |
| M4 | Imagens | ⚠️ **Refeitas**: 15 arquivos em `materiais-finais/criativos-corrigidos/` (1080×1080, 1080×1350, 1080×1920). O cliente sobe pela biblioteca de mídia; o ambiente não envia arquivos |
| M5 | Anúncios | 🚫 Dependem de M2, M3 e M4, e das correções das peças (`materiais-finais/correcoes-criativos.md`) |

## Antes de produzir/usar os criativos

| # | Pendência |
|---|---|
| 6 | Logotipo oficial (arquivo) |
| 7 | Manual de marca (cores e fontes oficiais) |
| 8 | Apresentador(a) e autorização de imagem e voz |
| 9 | ✅ Identificação: cliente autorizou `OAB/MT 16.113` nas artes (2026-10-24). Pendente: confirmar se deve vir com o nome do advogado responsável |
| 10 | Trilha sonora licenciada |
| 11 | Escolha dos criativos da fase 1 |
| 11a | Criativos já prontos: **revisados** (ver relatório). Pendente: corrigir C e D (aviso, zonas seguras), A (logotipo e aviso fora da faixa inferior), logotipo oficial em todas as peças, grafia única da marca (Correa × Corrêa), versões 1:1 e 4:5 faltantes. O criativo “escondidas” **continua não revisado** |
| 11b | **Landing page:** versão corrigida proposta em `materiais-finais/landing-revisao-veiculos_corrigida.html` (L1, L3, L4, L5, L6, L9, L10, L13 resolvidos no HTML). **Pendentes:** advogado aprovar o texto novo; publicar no Bitrix24; instalar pixel e evento `Lead` (L7); alcance geográfico (L8); revisar o vídeo (L11); grafia da marca (L12). Ver `materiais-finais/landing-alteracoes.md` |
| 11c | **Perguntas para o advogado responsável:** (a) depoimentos: o cliente informa que são reais e autorizados, mas **[Provável]** a norma de publicidade os veda e eles descrevem desfechos; ficam **fora** da versão corrigida até confirmação por escrito; (b) texto novo da landing, no lugar de “pacificado”/“consolidada”; (c) “Atuação em…” no lugar de “especializada”; (d) inscrição suplementar fora de MT, dado o alcance nacional da campanha |
| 11d | **Peças:** correções por peça em `materiais-finais/correcoes-criativos.md` (aviso, OAB, zonas seguras, perguntas impessoais, barras de E/F, CTA, formatos faltantes) |

## Antes de publicar

| # | Pendência |
|---|---|
| 12 | Definição de “lead qualificado” e metas numéricas (custo máximo por lead qualificado, taxa mínima de contato) |
| 13 | Como o lead chega ao Bitrix24 e em qual funil; campo de origem do lead |
| 14 | Equipe e prazo de primeiro contato para esta área (direito bancário/consumidor) |
| 15 | Tipo de formulário (“maior intenção” × “mais volume”). **O formulário nativo precisa ser criado no Gerenciador de Anúncios: não há ferramenta para criá-lo neste ambiente.** |
| 16 | Pergunta 2 do formulário: manter múltipla escolha com duas opções ou capturar o nome do banco |
| 17 | E-mail obrigatório ou não no formulário |
| 18 | Base legal e retenção de dados (LGPD) |
| 19 | Eventos de site (depende de instalar o pixel, item 5b) |
| 20 | Nome da campanha: forma mista ou em maiúsculas |
| 21 | Orçamento: CBO ou ABO; confirmação da divisão R$ 30 + R$ 20 |
| 22 | Disponibilidade de botões de CTA nativos no objetivo e nos posicionamentos escolhidos |
| 23 | Disponibilidade do posicionamento Threads na conta |
| 24 | Públicos de remarketing: nenhum existe na conta; criar e definir tamanho mínimo |
| 25 | Zonas seguras de Reels e Stories na orientação vigente da Meta |
| 26 | Teste futuro com todos os gêneros (precisa de autorização) |
| 27 | Limpeza da conta: 34 campanhas pausadas e duplicadas aumentam o risco de reativar uma por engano |

## Informações institucionais não inseridas

Número da OAB, endereço, telefone e e-mail institucionais não foram inseridos nos materiais. Os documentos do repositório (`docs/`) contêm dados de contato do site principal, mas **não foram usados** porque o briefing proíbe inserir dados institucionais não fornecidos para esta campanha. Se o cliente aprovar o uso, informar quais.
