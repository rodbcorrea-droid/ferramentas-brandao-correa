# Landing page corrigida — o que mudou

Arquivo proposto: `landing-revisao-veiculos_corrigida.html`. O original (`landing-revisao-veiculos.html`) **não foi alterado**.

**Isto é uma proposta.** O texto novo precisa ser aprovado pelo advogado responsável antes de ir ao ar. Nada foi publicado; este ambiente não alcança o Bitrix24.

## Itens da revisão

| Item | Antes | Agora | Estado |
|---|---|---|---|
| L1 | “Você Pode Ter Pago Juros Abusivos Sem Saber.” | “A taxa do contrato pode ser analisada.” + texto do briefing e a frase “Superar a média, isoladamente, não comprova abusividade” | ✅ |
| L2 | 3 depoimentos com 5 estrelas e desfechos | **Seção removida.** Em seu lugar, “O que ajuda na análise inicial” (veículo, banco, parcelas, situação). Um comentário no HTML marca o ponto de reinserção | ⏳ ver nota abaixo |
| L3 | Todo caminho do quiz termina em “Seu contrato pode ter direito à Revisão e Restituição!”; opção “parcelas em atraso” | Triagem neutra; resultado: “A equipe pode fazer uma análise inicial… não indica nem garante resultado”; opção de atraso removida | ✅ |
| L4 | “pacificado”, “Jurisprudência Consolidada”, “Até 10 Anos”, “inclusive já quitados”, “Venda Casada”, “Tema 972” | Removidos. Textos com “pode”, “conforme a documentação”, “depende do contrato” | ✅ (advogado deve revisar o texto novo) |
| L5 | “É muito comum os bancos embutirem…” | “O contrato pode prever seguros, tarifas e encargos. A análise verifica o que consta do documento…” | ✅ |
| L6 | Sem política de privacidade | Link no modal do formulário e no rodapé, com texto de uso dos dados; aviso padrão sob o botão e no rodapé | ✅ |
| L7 | `InitiateCheckout` ao abrir o formulário; sem pixel | Trocado pelo evento personalizado `FormularioAberto`. Comentário no `<head>` marca onde entra o código-base do pixel. **O evento `Lead` no envio do formulário continua pendente** (precisa do pixel e do evento de envio do Bitrix24) | ⏳ |
| L8 | “em Mato Grosso”, “em todo MT”, TJMT | Referências removidas. **OAB/MT 16.113 e Cuiabá/MT permanecem** (cabeçalho, bloco “Como funciona” e rodapé). A pergunta sobre inscrição suplementar fora de MT continua aberta | ⏳ |
| L9 | “Atuação especializada” | “Atuação em Direito Bancário e Defesa do Consumidor” | ✅ (confirmar) |
| L10 | Barra com ponto pulsante, botão pulsante, modal de saída, “Garantido” | Barra informativa estática; animações pulsantes e modal de saída removidos; “Sigilo profissional” | ✅ |
| L11 | Vídeo Vimeo | **Mantido; conteúdo não revisado** (comentário no HTML) | ⏳ |
| L12 | “Corrêa” × “Correa” | **Mantido “Corrêa” na página.** Decidir uma grafia para todas as peças | ⏳ |
| L13 | `meta description` com alegações | Reescrita com a copy do briefing | ✅ |

**Também alterado:** o rodapé deixou de afirmar “em estrita observância ao Provimento nº 205/2021”. É uma autodeclaração que este pacote não consegue verificar.

## Sobre os depoimentos (L2)

Você informou que são reais e autorizados. Isso resolve a autenticidade, mas **não** resolve se a norma de publicidade da advocacia permite exibi-los. **[Provável]** o Provimento 205/2021 veda depoimentos e divulgação de resultados. Os textos atuais também descrevem desfechos (“entrou com o pedido de restituição”), o que é um segundo problema.

Por isso a seção ficou **fora** da versão corrigida. Para reinserir: o advogado confirma por escrito que é permitido; os textos perdem qualquer menção a desfecho; o ponto de reinserção está marcado no HTML.

## Como foi verificado

- Estrutura HTML balanceada (sem tags abertas).
- Varredura de termos problemáticos (“abusivos sem saber”, “pacificado”, “venda casada”, “Tema 972”, “STJ”, “TJMT”, depoimentos, estrelas, “em atraso”, “enquadrado”, modal de saída): **nenhuma ocorrência** no HTML novo.
- Renderização em navegador sem rede, em celular (390 px) e computador (1200 px): sem erro de JavaScript; o quiz foi percorrido até o resultado.

**Não verificado:** o vídeo (Vimeo), o formulário do Bitrix24 e o comportamento com a página no ar. No teste, essas partes ficaram bloqueadas de propósito.

## Como colocar no ar

Substitua o conteúdo do bloco HTML da página `…/jurosfinan/` pelo arquivo corrigido. Teste no celular com a internet ligada: o formulário e o vídeo só carregam online. Depois, instale o pixel (comentário no `<head>`) e configure o evento `Lead` no envio.
