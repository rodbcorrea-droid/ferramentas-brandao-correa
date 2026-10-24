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
| 5c | Criativos prontos do cliente | ⏳ Fora do alcance | Há PNGs e um HTML de landing na pasta local do cliente (`CLAUDE CODE META ADS`). **Não estão no repositório nem neste ambiente.** Precisam ser enviados (ver README). Não foram revisados. |

## Antes de produzir/usar os criativos

| # | Pendência |
|---|---|
| 6 | Logotipo oficial (arquivo) |
| 7 | Manual de marca (cores e fontes oficiais) |
| 8 | Apresentador(a) e autorização de imagem e voz |
| 9 | Identificação profissional a exibir nas artes, se exigida pela revisão já feita |
| 10 | Trilha sonora licenciada |
| 11 | Escolha dos criativos da fase 1 |
| 11a | **Revisar os criativos já prontos** contra `conformidade/` antes de subir (um dos arquivos se chama “escondidas”; o nome sugere um apelo que o briefing proíbe, mas o conteúdo não foi visto) |

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
