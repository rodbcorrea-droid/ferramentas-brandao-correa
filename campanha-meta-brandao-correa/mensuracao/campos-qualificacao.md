# Campos de qualificação e planilha de acompanhamento

Estrutura para registrar cada lead no Bitrix24 ou em planilha. Nenhum campo exige CPF, RG, número do contrato ou dados bancários.

## 1. Campos

| Campo | Origem | Tipo | Valores / formato |
|---|---|---|---|
| ID do lead | Meta / CRM | texto | automático |
| Data e hora do lead | Meta | data/hora | |
| Nome | Formulário | texto | |
| Telefone | Formulário | texto | |
| E-mail | Formulário | texto | se coletado |
| Campanha | Meta | texto | |
| Conjunto | Meta | texto | |
| Anúncio (origem do criativo) | Meta | texto | nome padronizado |
| Origem regional | Meta (breakdown) ou DDD | lista | Sudeste, Sul, Centro-Oeste, Norte-Nordeste, N/A |
| Tipo de veículo | Pergunta 1 | lista | Carro, Moto |
| Banco ou financeira informado | Pergunta 2 | lista/texto | conforme o formulário final |
| Situação do contrato | Pergunta 3 | lista | Quitado, Em andamento |
| Quantidade de parcelas | Pergunta 4 | texto/número | aproximada |
| Data do primeiro contato | Equipe | data/hora | |
| Tempo até o primeiro contato | calculado | minutos | |
| Status do lead | Equipe | lista | ver abaixo |
| Resultado da triagem | Equipe | lista | Apto para análise, Não apto, Aguardando documentos, N/A |
| Motivo de perda | Equipe | lista | Sem contato, Sem interesse, Fora do escopo, Dado incorreto, Outro |
| Observações | Equipe | texto | não registrar dados sensíveis desnecessários |

## 2. Status do lead

1. Novo
2. Tentativa de contato
3. Contato efetuado
4. Triagem concluída — apto para análise
5. Triagem concluída — não apto
6. Aguardando documentos
7. Em análise
8. Convertido
9. Perdido (com motivo)

“Lead qualificado” = status 4 em diante, **conforme definição a confirmar com o cliente**.

## 3. Planilha de acompanhamento (colunas sugeridas por criativo e por conjunto)

| Coluna | Fonte |
|---|---|
| Período | |
| Campanha / Conjunto / Anúncio | Meta |
| Amount spent | Meta |
| Reach, Impressions | Meta |
| Link clicks, CTR (link) | Meta |
| Landing page views | Meta (se houver pixel) |
| Leads (Results) | Meta |
| Cost per result | Meta |
| Leads recebidos no CRM | CRM |
| Contato efetivo | CRM |
| Leads qualificados | CRM |
| Custo por lead qualificado | calculado: Amount spent ÷ leads qualificados |
| Convertidos | CRM |

Dado indisponível: “N/A” ou “Data not available”.

## 4. Privacidade

- Coletar o mínimo necessário.
- Definir quem acessa os leads e por quanto tempo são mantidos (LGPD, a confirmar).
- Não exportar leads para ferramentas sem finalidade definida.
