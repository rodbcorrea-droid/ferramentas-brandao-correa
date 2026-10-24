# Plano de otimização

Este plano não contém previsões de desempenho. Os limiares de decisão em números (custo máximo por lead qualificado, taxa mínima de contato) devem ser definidos com o cliente **antes** do lançamento (**a confirmar**).

## Princípio

Otimizar pelo **custo por lead qualificado** e pelo **aproveitamento comercial**, não pelo menor custo por lead. O custo por lead isolado pode premiar leads fracos.

## Fases

### Fase 0 — Pré-lançamento
- Resolver as pendências de `../pendencias-a-confirmar.md`.
- Definir o que é “lead qualificado” e a forma de registrar (ver `../mensuracao/campos-qualificacao.md`).
- Preparar o fluxo de atendimento e o prazo de primeiro contato.
- Escolher os criativos da fase 1 (pouco material, bem revisado).

### Fase 1 — Aprendizado (primeiros 7 dias)
- Não editar orçamento, público ou criativos dos conjuntos sem necessidade. Edições reiniciam ou prolongam o aprendizado.
- Primeiras 72 horas: conferir aprovação, entrega, formulário, recebimento de leads e UTMs. Não avaliar desempenho.
- Ler **cada lead** recebido nos primeiros dias para checar se as respostas fazem sentido.

### Fase 2 — Leitura
- Compare por **lead qualificado**, não por lead.
- Aplique a matriz de testes (`matriz-testes-ab.md`), um teste por vez.
- Registre cada decisão e o motivo.

### Fase 3 — Consolidação e expansão
- Consolidar conjuntos com público sobreposto ou pouco volume.
- Separar Sul e Centro-Oeste, ativar o conjunto 4 e o teste com todos os gêneros apenas com autorização e orçamento.

## Regras de decisão

1. Não declarar vencedor com resultado isolado ou de poucos dias.
2. Não pausar um anúncio apenas por custo inicial alto sem olhar a qualidade dos leads.
3. Alterações de orçamento em passos pequenos (regra prática comum: até cerca de 20% por vez; **a confirmar**).
4. Uma variável por vez.
5. Reprovação de anúncio: não republicar o mesmo texto; revisar com `../conformidade/`.
6. Frequência alta e queda de CTR (link) indicam desgaste: trocar criativo antes de aumentar orçamento.
7. Dado indisponível: registrar “N/A” ou “Data not available”. Não preencher com estimativas.

## Rotina

| Periodicidade | Ação |
|---|---|
| Diária (fase 1) | Conferir entrega, reprovações, leads recebidos e tempo de resposta |
| Semanal | Atualizar a planilha de acompanhamento; comparar por lead qualificado; decidir um ajuste |
| Quinzenal | Revisar exclusões de remarketing; revisar fadiga de criativo |
| Mensal | Revisar objetivos, orçamento e plano de testes |

## Sinais e possíveis causas (hipóteses a verificar, não conclusões)

| Sinal | Possível causa | Onde verificar |
|---|---|---|
| Muitas aberturas e poucos envios do formulário | Formulário longo, pergunta confusa, expectativa diferente do anúncio | Taxa de abertura × conclusão |
| Leads com telefone inválido ou respostas aleatórias | Formulário de “mais volume”, posicionamento de baixa intenção | Qualidade por posicionamento e tipo de formulário |
| Muitos leads de “Não lembro” em tudo | Pergunta do banco em múltipla escolha | `../formulario-meta.md` |
| CTR (link) baixo | Gancho fraco ou criativo desgastado | Criativos e frequência |
| Leads bons de um conjunto e ruins de outro | Região ou público | Origem regional, `../mensuracao/campos-qualificacao.md` |
| Anúncio reprovado | Texto sugere atributo pessoal ou promessa | `../conformidade/checklist-meta.md` |
