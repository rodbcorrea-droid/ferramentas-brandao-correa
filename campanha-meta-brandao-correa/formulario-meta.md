# Formulário nativo do Meta Ads

Documentação do formulário. Não foi criado em nenhuma conta. Versão estruturada em `dados/formulario-meta.json` (somente documentação).

## 1. Identificação

| Campo | Conteúdo |
|---|---|
| Nome interno | Qualificação \| Juros Financiamento Carro e Moto |
| Título de apresentação | Entenda o seu financiamento |
| Descrição | Responda às perguntas sobre o financiamento do seu carro ou moto. A análise depende do contrato e das circunstâncias do caso. Não há promessa de resultado. |
| Tipo de formulário | **A confirmar.** Sugestão: “maior intenção” (com tela de revisão), para reduzir leads acidentais. |

## 2. Perguntas

**Pergunta 1 — O que foi financiado?**
Tipo: múltipla escolha. Respostas: Carro; Moto.

**Pergunta 2 — Qual banco ou financeira aparece no contrato?**
Tipo: múltipla escolha, conforme o briefing. Respostas: “Banco ou financeira informado no contrato”; “Não lembro”.

> **Atenção.** Com estas duas opções, a resposta **não registra o nome do banco**. Para a triagem, o nome é a informação útil. Alternativas a decidir (a confirmar): (a) campo de resposta curta; (b) lista com as principais instituições + “Outro” + “Não lembro”. O formulário foi documentado exatamente como solicitado; a alternativa não foi aplicada.

**Pergunta 3 — O financiamento já está quitado?**
Tipo: múltipla escolha. Respostas: “Sim, já está quitado”; “Não, ainda estou pagando”.

**Pergunta 4 — Você lembra quantas parcelas foram contratadas? Informe uma quantidade aproximada.**
Tipo: resposta livre.

## 3. Informações de contato

- Nome completo.
- Telefone.
- E-mail, **se necessário para a operação** (a confirmar).

Não exigir verificação por SMS se o campo de telefone não estiver obrigatório e corretamente configurado.

## 4. Mensagem de uso dos dados

> Usaremos seus dados para analisar as informações do financiamento e entrar em contato sobre a solicitação. Consulte a política de privacidade da Brandão Correa Assessoria Jurídica.

- Link da política de privacidade: `https://brandaocorrea.bitrix24.site/politica/` (informado em 2026-10-24; a Meta exige uma URL válida no formulário). **Conferir que a página abre e cobre esta finalidade**; não foi possível abri-la a partir do ambiente do pacote.
- Base legal e finalidade (LGPD): **a confirmar** com o responsável pela proteção de dados do escritório.

## 5. Tela de conclusão

| Campo | Conteúdo |
|---|---|
| Título | Recebemos suas informações |
| Descrição | A equipe da Brandão Correa Assessoria Jurídica fará uma análise inicial das informações e poderá entrar em contato pelo telefone informado. O preenchimento não garante resultado ou contratação. |
| CTA | Saiba mais |
| Link | https://acidentesinss.bitrix24.site/jurosfinan/ |

## 6. O que não fazer

- Não ativar códigos promocionais.
- Não solicitar CPF, RG, número completo do contrato, dados bancários ou documentos sensíveis no formulário inicial.
- Não adicionar perguntas além das quatro acima.
- Não alterar o texto das perguntas sem registrar a mudança.

## 7. Teste antes de publicar

- [ ] Prévia do formulário no celular.
- [ ] Envio de lead de teste e conferência do recebimento.
- [ ] Integração com o Bitrix24 (ou rotina de download) funcionando.
- [ ] Alerta de novo lead para a equipe de atendimento.
- [ ] Política de privacidade abrindo.
- [ ] Landing page da tela final abrindo no celular.
