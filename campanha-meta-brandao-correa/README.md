# Campanha Meta Ads — Brandão Correa Assessoria Jurídica

**Tema:** análise de contratos de financiamento de carros e motos
**Gerado em:** 2026-10-24
**Status:** pacote de documentação. **Nada foi publicado, ativado, pago, enviado ou criado em conta alguma.** Nenhuma imagem ou vídeo foi gerado. Nenhuma credencial foi usada.

> A campanha deve permanecer em **rascunho/pausada** até a autorização final e manual. Antes disso, resolva as pendências de `pendencias-a-confirmar.md`.

## Decisões do cliente (2026-10-24)

| Tema | Decisão |
|---|---|
| Público | Prosseguir com **homens, 22+**, mesmo havendo risco de a Meta restringir gênero e idade. Se a restrição aparecer na configuração, usar o que a Meta permitir e registrar. **Não contornar.** |
| Regras da OAB | Revisadas pelo cliente. Este pacote não verificou essa revisão. |
| Landing page | `https://acidentesinss.bitrix24.site/jurosfinan/` (substitui a `.../2684/` do briefing original) |
| Política de privacidade | `https://brandaocorrea.bitrix24.site/politica/` |
| Conta de anúncios | `1155384176705579` (nome na listagem anterior: “SALÁRIO MATERNIDADE - DR.RODRIGO BRANDÃO”, moeda BRL) |

## Achados da conta `1155384176705579` (consulta em 2026-10-24)

Acesso autorizado pelo cliente. Foi feita **somente leitura**: nada foi criado, alterado ou publicado.

| Item | Achado |
|---|---|
| Página do Facebook | “Brandão Correa Assessoria Jurídica” (`2033836416865143`) |
| Instagram | `@brandaocorrea.adv` (`17841407573996167`) |
| **Termos de lead ads** | **A API informa que a Página NÃO aceitou** (`leadgen_tos_accepted = false`). Aceitar em https://www.facebook.com/legal/leadgen/tos antes de criar o conjunto de anúncios. **Bloqueia a criação.** |
| **Pixel de site** | **Nenhum.** O único dataset é “WhatsApp Marketing Message Event Sharing”. Sem pixel na landing page não há *Landing page views* nem remarketing por visita ao site. |
| Públicos personalizados | Nenhum. Os públicos de remarketing precisam ser criados do zero. |
| Campanhas existentes | 34, **todas pausadas e sem gasto nos últimos 30 dias** (inclui “[TESTE] [RASCUNHO] [NÃO PUBLICAR]” e várias cópias). A conta está sem histórico recente de entrega. |

**Ainda não verificado:** as duas páginas (landing e política) não puderam ser abertas a partir do ambiente em que o pacote foi montado (domínio bloqueado pela rede). O domínio da landing, `acidentesinss`, difere do domínio `inssacidentes` usado em todos os documentos do repositório. **Confirmar que a URL está correta** (pode ser outro site ou erro de digitação).

## Materiais recebidos e revisados (2026-10-24)

Foram recebidos 5 imagens (4 distintas) e o HTML da landing. Estão em `materiais-finais/`; a revisão completa está em `conformidade/revisao-materiais-2026-10-24.md`.

| Material | Veredito |
|---|---|
| Landing page | **Reprovada**: 3 problemas bloqueantes (afirmação “você pode ter pago juros abusivos”, depoimentos com estrelas, quiz que dá o mesmo resultado positivo a todos) |
| Criativo B (4:5) | Quase pronto |
| Criativo A (9:16) | Aprovável após reposicionar logotipo e aviso |
| Criativos C e D (9:16) | **Não publicar**: sem aviso jurídico |

**Não recebidos:** versões 1:1 e o criativo “escondidas”. Nada foi enviado ao Meta.

---

## 1. Objetivo

Gerar leads qualificados por **formulário nativo** do Meta Ads, com triagem inicial do financiamento (veículo, banco ou financeira, situação do contrato, parcelas), sem prometer resultado jurídico ou econômico.

## 2. Público

Configuração inicial solicitada: **homens, a partir de 22 anos (22 a 65+)**, que moram nas regiões escolhidas. Contratos em andamento e quitados. Detalhes, sugestões de interesses e testes em `estrategia-publicos.md`.

Observação: a configuração por gênero e idade pode **não estar disponível** se a Meta exigir categoria especial de anúncio para esta campanha. O cliente decidiu prosseguir mesmo assim; ver `conformidade/checklist-meta.md`.

## 3. Regiões

| Conjunto | Estados |
|---|---|
| Sudeste | SP, RJ, MG, ES |
| Sul | PR, SC, RS |
| Centro-Oeste | MT, MS, GO, DF |
| Norte-Nordeste (ou Brasil excluindo as regiões acima) | opção da fase 3 |

## 4. Orçamento

R$ 50,00 por dia no total. Para evitar fragmentação, a recomendação da fase 1 é **Sudeste R$ 30,00 + demais regiões R$ 20,00** (Sul e Centro-Oeste unificados). Ver `estrategia-publicos.md`.

## 5. Estrutura

Campanha `LEADS | Financiamento Veículos | Análise Contratual | BR` → 4 conjuntos regionais (2 ativos na fase 1) → anúncios por formato. Modelo em `dados/estrutura-campanha.json` (somente documentação; não enviar à API).

## 6. Formulário

`formulario-meta.md` e `dados/formulario-meta.json`. Quatro perguntas, contato, mensagem de uso dos dados e tela de conclusão. Sem CPF, RG, número do contrato, dados bancários ou documentos.

## 7. Landing page

`https://acidentesinss.bitrix24.site/jurosfinan/` — usada na tela final do formulário e como destino complementar. **Não foi possível verificar o conteúdo desta página** (domínio bloqueado pela rede do ambiente). Revise-a com `conformidade/checklist-publicidade-juridica.md` antes de usá-la. Páginas anteriores do cliente (pasta `docs/`) usam linguagem que contraria este briefing (promessa de valor, urgência, depoimentos).

## 8. Criativos necessários (todos a produzir manualmente)

| Tipo | Quantidade | Formatos | Arquivo de especificação |
|---|---|---|---|
| Reels 15 s | 5 | 9:16 (+ 4:5 e 1:1) | `roteiros/reels-15-segundos.md` |
| Reels 30 s | 5 | 9:16 (+ 4:5 e 1:1) | `roteiros/reels-30-segundos.md` |
| Reels 45 s | 3 | 9:16 (+ 4:5 e 1:1) | `roteiros/reels-45-segundos.md` |
| Stories (5 quadros) | 5 | 9:16 | `roteiros/stories.md` |
| Estáticos | 8 | 1:1, 4:5, 9:16 | `criativos/especificacoes-estaticos.md` |
| Carrosséis (5 cards) | 3 | 1:1 | `criativos/carrosseis.md` |

Total: 29 criativos planejados (lista completa em `dados/nomes-criativos.csv`). Na fase 1, com R$ 50/dia, **não produza nem publique todos**. Ver `testes/plano-otimizacao.md`.

## 9. Como inserir os criativos manualmente

Os passos abaixo descrevem o fluxo no Gerenciador de Anúncios. Nomes de menus podem mudar (a confirmar).

1. Entre no Gerenciador de Anúncios, na conta de anúncios `1155384176705579`. A **Página do Facebook e o perfil do Instagram** a vincular ainda estão **a confirmar**.
2. Crie a campanha com objetivo **Leads** e local de conversão **Formulários instantâneos**. Use o nome e o orçamento de `dados/estrutura-campanha.json`.
3. Antes de continuar, defina a **categoria especial de anúncio** (ver `conformidade/checklist-meta.md`).
4. Crie o conjunto 1 (Sudeste): localização "pessoas que moram nesta localização", idade, gênero, público (A ou B) e posicionamentos Advantage+.
5. Crie o formulário conforme `formulario-meta.md` e teste a **prévia**.
6. Crie os anúncios: envie **manualmente** os arquivos nos formatos 9:16, 4:5 e 1:1; cole texto principal, título, descrição e CTA de `copies/`; configure a tela de conclusão com a landing page; adicione os parâmetros de `mensuracao/utms.md`.
7. Confira a prévia em cada posicionamento (Reels, Stories, Feed).
8. Salve como **rascunho** ou mantenha **pausado**. Não clique em publicar.

## 10. Como nomear os arquivos

- Nome do anúncio: `FORMATO | CONCEITO | ÂNGULO | VERSÃO`, por exemplo `REELS | TAXA MÉDIA | EDUCATIVO | V01`.
- Nome do arquivo: coluna `arquivo_sugerido` de `dados/nomes-criativos.csv`, por exemplo `reels_taxa-media_educativo_v01_9x16_15s.mp4`.
- Regras completas em `mensuracao/nomes-padroes.md`.

## 11. Revisão antes da publicação

Use `checklist-final-publicacao.md`, `conformidade/checklist-meta.md`, `conformidade/checklist-publicidade-juridica.md` e `criativos/checklist-producao.md`. Nenhum item pendente pode ficar sem responsável.

## 12. Como interpretar os primeiros resultados

- Nas primeiras 72 horas, verifique **aprovação dos anúncios, entrega e funcionamento do formulário**. Não avalie desempenho.
- Durante a primeira semana, não conclua por custo. Leia os leads recebidos um a um e compare o custo por **lead qualificado**, não apenas por lead.
- Declare vencedor apenas conforme `testes/matriz-testes-ab.md`.
- Métricas e definições em `mensuracao/metricas.md`. Dado indisponível deve ser registrado como “N/A” ou “Data not available”.

## 13. O que não deve ser publicado

- Qualquer frase de `conformidade/frases-proibidas-e-substituicoes.md`.
- Taxas, percentuais, valores, depoimentos, nomes de bancos, OAB, endereço ou telefone que não tenham sido fornecidos e aprovados.
- Imagens ou vídeos que acusem bancos ou sugiram que a pessoa está endividada, enganada ou lesada.
- A landing page, se ela não passar na revisão.

## 14. A campanha permanece pausada

Sim. Publicação depende de aprovação manual e de todos os itens de `checklist-final-publicacao.md` resolvidos.

## 15. Índice de arquivos

```
campanha-meta-brandao-correa/
├── README.md
├── briefing-campanha.md
├── estrategia-publicos.md
├── posicionamentos.md
├── formulario-meta.md
├── checklist-final-publicacao.md
├── pendencias-a-confirmar.md
├── copies/            (copies-principais, institucionais, educativas, contrato-quitado, remarketing, titulos-e-descricoes)
├── roteiros/          (reels-15, reels-30, reels-45, stories)
├── criativos/         (especificacoes-estaticos, carrosseis, prompts-visuais, checklist-producao, instrucoes-designer, instrucoes-editor-video)
├── testes/            (matriz-testes-ab, plano-otimizacao)
├── mensuracao/        (utms, nomes-padroes, campos-qualificacao, metricas)
├── conformidade/      (checklist-meta, checklist-publicidade-juridica, frases-proibidas-e-substituicoes)
└── dados/             (copies.csv, roteiros.csv, nomes-criativos.csv, estrutura-campanha.json, formulario-meta.json)
```

Os CSV usam **ponto e vírgula** como separador e codificação UTF-8 com BOM (abrem corretamente no Excel em português). Os JSON são apenas documentação.

## 16. Pendências

Tudo o que não foi fornecido está marcado como **“a confirmar”** e consolidado em `pendencias-a-confirmar.md`.
