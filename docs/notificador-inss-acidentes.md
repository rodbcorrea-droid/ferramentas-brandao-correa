# Notificador INSS Acidentes
## URL: https://inssacidentes.bitrix24.site/notificador/

### O que faz:
Sistema de notificação extrajudicial para o escritório Brandão Correa Assessoria Jurídica, integrado com Bitrix24.

### Fluxo (5 etapas):

#### 1. Upload de Documentos
- **Contrato ZapSign** (PDF) — modelo identificado automaticamente
- **Boleto Bancário** (PDF) — opcional, fallback para Asaas/Bitrix24

#### 2. Tipos de Notificação
| Classe | Tipo | Descrição |
|--------|------|-----------|
| Cl. 2 | Pagamento | Cobrança de Honorários Advocatícios — prazo 5 dias úteis após saque. Multa 1 URH + juros 1%/mês + INPC |
| Cl. 5 | Multa Contratual | Rescisão e Multa — inadimplemento/desistência/revogação |
| Cl. 5.1 | MEU INSS | Violação de Senha/Duplo Fator — multa R$ 250,00 por ocorrência |
| Cl. 7 | Mora Automática | Constituição em Mora — art. 397 CC |
| Doc. | Certidão Nascimento | Solicitação de documentação para instrução do pedido |

#### 3. Dados das Partes
- **Notificado (Contratante):** Nome, CPF, RG, Estado Civil, Profissão, E-mail, Celulares, Endereço, Nº Processo, Benefício, Valor em Aberto, Data, ID Bitrix24
- **Notificantes (Contratados):** Advogados (1-3), Endereço Profissional, Telefone, E-mail, Website, Foro Eleito

#### 4. Análise de Autenticidade ZapSign
- Verificação dos pontos de autenticação
- Compara dados do signatário no relatório ZapSign com cadastro do contrato

#### 5. Configurações & Disparo
**Integrações Bitrix24:**
- ID Responsável (Karina — ID 4)
- ID Grupo FATURA/FINANCEIRO
- ID Fila Robocall (TELEFONES PRIMEIRO — ID 17)
- Linha WhatsApp (app/165)
- ID Pasta Drive CLIENTES (ID 1697545)

**Ações de Disparo:**
- ☁️ Drive Bitrix24
- 📧 E-mail CRM
- 📱 SMS
- 💬 WhatsApp
- 📞 Robocall + Fila
- 📋 Tarefa CRM

### Integrações:
- Bitrix24 (CRM, Drive, Tarefas, Robocall)
- ZapSign (verificação de autenticidade)
- Asaas (cobrança/boleto)
- WhatsApp (via Bitrix24 app/165)
