# Checklist final de publicação

**Estado em 2026-10-24:** nada foi criado, enviado ou publicado em conta alguma.

Legenda: ✅ atendido na documentação (conferido por varredura automática do texto e leitura) · ⏳ **PENDENTE** (depende de ação manual) · ⚠️ **ATENÇÃO** (atendido em parte; ler a nota).

Itens ✅ valem para o **texto do pacote**. Eles precisam ser revistos de novo sobre as peças finais produzidas.

## Configuração

- [ ] ⏳ **PENDENTE** Página correta selecionada. (Conta `1155384176705579`; Página `2033836416865143`; Instagram `@brandaocorrea.adv`. **Termos de lead ads não aceitos segundo a API: aceitar antes de criar.**)
- [ ] ⏳ **PENDENTE** Campanha com objetivo Leads. (Documentada em `dados/estrutura-campanha.json`; não criada.)
- [ ] ⏳ **PENDENTE** Orçamento revisado. (R$ 50/dia; divisão e tipo CBO/ABO a confirmar.)
- [ ] ⏳ **PENDENTE** Regiões revisadas.
- [ ] ⏳ **PENDENTE** Idade revisada. ⚠️ Cliente decidiu prosseguir com 22+; conferir o que a Meta permite na configuração.
- [ ] ⏳ **PENDENTE** Gênero revisado. ⚠️ Cliente decidiu prosseguir com homens; conferir o que a Meta permite na configuração.

## Formulário

- [ ] ⏳ **PENDENTE** Formulário correto selecionado.
- [ ] ⏳ **PENDENTE** Pergunta sobre carro ou moto revisada.
- [ ] ⏳ **PENDENTE** Pergunta sobre banco revisada. ⚠️ Com duas opções fixas, o nome do banco não é capturado (`formulario-meta.md`).
- [ ] ⏳ **PENDENTE** Pergunta sobre quitação revisada.
- [ ] ⏳ **PENDENTE** Pergunta sobre parcelas revisada.
- [ ] ⏳ **PENDENTE** Política de privacidade preenchida. (URL informada: `https://brandaocorrea.bitrix24.site/politica/`; falta inserir no formulário e conferir que abre.)
- [ ] 🚫 **REPROVADA NA REVISÃO** Landing page testada. Revisada em 2026-10-24: 3 itens bloqueantes (`conformidade/revisao-materiais-2026-10-24.md`). **Versão corrigida proposta** em `materiais-finais/landing-revisao-veiculos_corrigida.html`; ainda precisa de aprovação do advogado, publicação, pixel e evento `Lead`. A página no ar continua reprovada. (`https://acidentesinss.bitrix24.site/jurosfinan/` não foi verificada; confirmar o domínio, que difere do `inssacidentes` usado no repositório.)
- [ ] ⏳ **PENDENTE** Formulário testado em modo de prévia.
- [ ] ⏳ **PENDENTE** Leads serão recebidos corretamente. (Integração com o Bitrix24 a definir.)

## Criativos

- [ ] ⏳ **PENDENTE** Criativos manuais inseridos. (4 criativos recebidos e revisados; nenhum enviado ao Meta; nenhum pronto para envio.)
- [ ] ⚠️ **ATENÇÃO** Versões 9:16, 4:5 e 1:1 revisadas. Faltam 1:1 de A, B e C e 4:5 de A, C, D e E (2ª remessa: E tem 1:1 e 9:16; D tem 1:1 e 9:16).
- [ ] ⏳ **PENDENTE** Legendas revisadas.
- [ ] ⚠️ **ATENÇÃO** Aviso jurídico revisado. Criativos C, D e E/F **não têm aviso**; no A o aviso está na faixa inferior coberta pela interface.

## Conformidade do conteúdo

- [ ] ⚠️ **ATENÇÃO** Nenhuma promessa de resultado. ✅ nas copies, roteiros e especificações do pacote (varredura sem ocorrências). ⚠️ **Na landing do cliente não**: o quiz termina em “Seu contrato pode ter direito à Revisão e Restituição!” para todas as respostas (L3) e o texto diz “entendimento pacificado” (L4).
- [x] ✅ Nenhuma taxa fictícia.
- [x] ✅ Nenhum percentual inventado. (Sem números seguidos de “%” nos materiais.)
- [ ] ⚠️ **ATENÇÃO** Nenhum depoimento inventado. ✅ no pacote. ⚠️ **A landing do cliente tem 3 depoimentos com 5 estrelas** (L2). Confirmar se são reais e autorizados; mesmo assim, recomendo remover.
- [x] ✅ Nenhum dado pessoal exposto. (Pacote sem OAB, endereço, telefone ou documento. Observação: a landing do cliente exibe “OAB/MT 16.113”; este pacote não a copiou nem validou.)
- [x] ✅ Nenhuma imagem sensacionalista. (Nenhuma imagem foi criada; as especificações proíbem o tipo.)
- [ ] ⚠️ **ATENÇÃO** Nenhuma frase que implique conhecimento da situação financeira da conta. As copies **P01** e **P11** abrem com pergunta dirigida à pessoa (“Financiou carro ou moto?”, “Você sabe qual era a taxa média…”). P01 contém a mensagem central do briefing. Revisar contra a política de atributos pessoais ou usar as versões impessoais (`dados/copies.csv`, coluna `atencao_atributos_pessoais`).

## Operação

- [ ] ⏳ **PENDENTE** Atendimento preparado para responder rapidamente. (Equipe e prazo a definir.)
- [x] ✅ Campanha ainda está pausada. (Não foi criada em nenhuma conta.)
- [x] ✅ Publicação depende de aprovação manual.

## Placar

| Situação | Itens |
|---|---|
| ✅ Atendidos | 6 |
| ⚠️ Atenção | 5 |
| 🚫 Reprovado na revisão | 1 (landing page) |
| ⏳ Pendentes | 17 |

**Os itens pendentes bloqueiam a publicação.** Os bloqueantes de decisão estão em `pendencias-a-confirmar.md` (itens 1 a 5).
