# Dashboard Financeiro — Drogaria Van Popular (SPA)
## URL: https://drogavanpopular.bitrix24.site/testes_ggsu/
## Título: "Resumo Financeiro Claude"

### Descrição:
Painel de controle financeiro (SPA) integrado com Bitrix24 CRM, provavelmente para um escritório de advocacia ou assessoria jurídica.

### Painéis:

#### 1. Controle de Pagamentos Mensais
- **Recebidos** — Pagamentos confirmados
- **Aguardando** — Pendentes
- **Em Atraso** — Vencidos
- **Ticket Médio** — Por recebimento
- **Total Honorários** — Soma do mês
- **Total Clientes** — Registros no mês

#### 2. Painel de Acordos
- Negócios tipo "Acordo Extrajudicial" + parcelas marcadas como acordo
- Total Acordos, Valor Total, Recebidos, Pendentes

#### 3. Painel de Inadimplência
- Inadimplentes ativos (não quitados)
- Regularizados (pagos após atraso)
- Valor em aberto total
- Média de dias em atraso
- Ordenação por: Data, Valor, Dias atraso

#### 4. Resumo 2026
- Consolidado mensal e totais do ano
- Total Recebido, Total em Atraso, Total Honorários, Total Clientes

### Configurações Bitrix24:
- **Método de Conexão:** CORS proxy (para chamadas de navegador)
- **SPA entityTypeId:** 1130
- **Category SPA0:** todas

### Mapeamento de Campos Bitrix24:
| Campo | Entidade | Campo Bitrix24 |
|---|---|---|
| Nº Pasta (principal) | CONTACT | UF_CRM_1726587995894 |
| Nº Pasta (fallback) | CONTACT | UF_CRM_1728598618 |
| Nome Completo | CONTACT | NAME + LAST_NAME |
| Tipo de Processo | SPA 1130 | ufCrm45_1758724694 |
| Parcela (atual/total) | SPA 1130 | ufCrm45_1757341060 / ufCrm45_1757341045 |
| Data de Pagamento | SPA 1130 | ufCrm45_1757341257 |
| Valor a Receber | SPA 1130 | ufCrm45_1757686357 |
| Honorários % | SPA 1130 | ufCrm45_1758725658 |
| Pago (fatura paga) | SPA 1130 | stageId = "Fatura Paga" (auto-detectado) |

### Estágios detectados:
- **"Fatura Paga"** — estágio de pagamento confirmado

### Notas:
- SPA = Single Page Application (painel dinâmico)
- Integra com Bitrix24 via API REST
- Usa proxy CORS para chamadas do navegador
- Provavelmente usado por Rod para controle financeiro do escritório
- Bitrix24 conta separada (drogavanpopular.bitrix24.site — diferente do inssacidentes)
