# Checklist de conformidade — Meta

Este checklist não substitui a leitura das políticas vigentes da Meta. Itens marcados **(a confirmar)** dependem do texto atual da política ou da configuração da conta.

## 1. Decisão que precisa vir antes de montar a campanha

### 1.1 Categoria especial de anúncio

**[Provável]** A Meta exige que anunciantes declarem “categorias especiais de anúncio” quando o anúncio se enquadra em determinados temas (como produtos e serviços financeiros). Quando a categoria se aplica, a segmentação é restrita (por exemplo, gênero e idade) e podem existir regras adicionais.

**Pergunta a responder (a confirmar):** um anúncio de **análise jurídica de contrato de financiamento** é um anúncio de produto/serviço financeiro? O escritório não oferece crédito, mas o tema é crédito e financiamento.

**Como decidir:** ler a política vigente de categorias especiais, conferir como o Gerenciador de Anúncios trata o caso e, se necessário, consultar o suporte da Meta. Registrar a decisão e a data.

**Consequências:**

| Decisão | Efeito |
|---|---|
| Declarar a categoria | Gênero e idade podem ficar indisponíveis. Como o público agora é **todos os gêneros**, 22+, o impacto prático é menor. |
| Não declarar | Risco de reprovação ou restrição da conta se a Meta entender que a categoria se aplicava. |

- [x] Decisão registrada: o cliente decidiu **prosseguir com o público solicitado** (2026-10-24).
- [ ] Na configuração real: registrar aqui o que a Meta efetivamente permitiu (gênero, idade, categoria declarada) e a data. Se a Meta bloquear, usar o permitido e avisar o cliente. Não contornar.

## 2. Atributos pessoais e situação financeira

- [ ] Nenhum texto afirma ou sugere que a pessoa está endividada, inadimplente, enganada ou em dificuldade financeira.
- [ ] Nenhuma pergunta de abertura sugere um atributo pessoal sensível. As copies que começam com “Financiou…”, “Você…” ou “Quitou…” estão marcadas em `dados/copies.csv` (`atencao_atributos_pessoais`) e precisam de revisão final. **Alternativa mais segura:** versões impessoais, já incluídas em `copies/`.
- [ ] A segmentação não usa critérios que impliquem situação financeira vulnerável.
- [ ] O formulário não pede dados sensíveis.

## 3. Alegações e conteúdo

- [ ] Nenhuma promessa de resultado, ganho ou prazo.
- [ ] Nenhuma taxa, percentual ou valor fictício.
- [ ] Nenhum depoimento ou resultado inventado.
- [ ] Nenhum nome ou logotipo de banco ou financeira sem autorização.
- [ ] Nenhum antes/depois, urgência artificial ou escassez falsa.
- [ ] Referência ao Banco Central apenas como fonte de “média de mercado divulgada”, sem usar brasão ou imagem oficial e sem sugerir parceria ou aval.
- [ ] Nenhuma aparência de anúncio governamental.

## 4. Formulário de leads

- [ ] URL da política de privacidade informada: `https://brandaocorrea.bitrix24.site/politica/`. **Conferir que abre** e cobre a finalidade. Não foi possível abri-la a partir do ambiente do pacote.
- [ ] Mensagem de uso dos dados exibida.
- [ ] Sem solicitação de CPF, RG, número do contrato, dados bancários ou documentos.
- [ ] Sem códigos promocionais.
- [ ] Sem verificação por SMS não configurada.
- [ ] Prévia testada.
- [ ] Lead de teste recebido.

## 5. Landing page

- [ ] Página abre em celular e carrega rápido.
- [ ] O conteúdo é coerente com o anúncio e com o formulário.
- [ ] Sem promessas, sem urgência artificial, sem depoimentos ou resultados não autorizados.
- [ ] Política de privacidade acessível.
- [ ] Identificação do escritório conforme a regra aplicável **(a confirmar)**.

## 6. Criativos

- [ ] Dentro das zonas seguras de Reels e Stories.
- [ ] Texto da arte curto e legível.
- [ ] Sem marca de banco, placa legível ou documento real.
- [ ] Sem imagens sensacionalistas.
- [ ] Aviso curto presente em todas as peças.

## 7. Conta e Página

- [x] Conta de anúncios definida pelo cliente: `1155384176705579`. Conferir, antes de criar, que está ativa, com forma de pagamento e sem restrição.
- [x] Página do Facebook (`2033836416865143`) e Instagram (`@brandaocorrea.adv`) vinculados à conta (consulta de 2026-10-24).
- [ ] 🚫 **Termos de lead ads aceitos na Página.** A API retornou `leadgen_tos_accepted = false`. Aceitar em https://www.facebook.com/legal/leadgen/tos antes de criar o conjunto.
- [ ] Pixel de site instalado na landing page. Hoje a conta só tem o dataset de WhatsApp.
- [ ] Forma de pagamento ativa.
- [ ] Sem restrição ou desativação pendente na conta. Observação: o histórico da conta do cliente indicou contas desativadas por “atividade incomum” em outro contexto. Confirmar que a conta escolhida está regular antes de investir produção.

## 8. Remarketing

- [ ] Públicos criados somente a partir de fontes permitidas.
- [ ] Listas de CRM, se usadas, têm base legal (LGPD) **(a confirmar)**.
- [ ] Textos não revelam que a plataforma sabe que a pessoa viu, visitou ou abandonou algo.
- [ ] Exclusões configuradas.
