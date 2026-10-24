# Padrões de nome

## 1. Campanha

Nome definido no briefing (seção de estrutura):

```
LEADS | Financiamento Veículos | Análise Contratual | BR
```

O briefing também apresenta a forma em maiúsculas (`LEADS | FINANCIAMENTO VEÍCULOS | ANÁLISE CONTRATUAL | BR`) no padrão de nomes. **A confirmar qual será usada.** Escolher uma só e manter em todos os relatórios.

## 2. Conjunto

```
REGIÃO | GÊNERO | IDADE | PÚBLICO
```

Exemplos:

```
SUDESTE | HOMENS | 22+ | AMPLO ADVANTAGE+
SUDESTE | HOMENS | 22+ | INTERESSES SUGERIDOS
SUL+CENTRO-OESTE | HOMENS | 22+ | AMPLO ADVANTAGE+
NORTE-NORDESTE | HOMENS | 22+ | AMPLO ADVANTAGE+
```

## 3. Anúncio

```
FORMATO | CONCEITO | ÂNGULO | VERSÃO
```

Exemplo:

```
REELS | TAXA MÉDIA | EDUCATIVO | V01
```

| Campo | Valores usados |
|---|---|
| FORMATO | REELS, STORIES, ESTÁTICO, CARROSSEL |
| CONCEITO | TAXA MÉDIA, QUITADO, CHECKLIST, VALOR DA PARCELA, EDUCAÇÃO FINANCEIRA |
| ÂNGULO | EDUCATIVO, PERGUNTA, INSTITUCIONAL (e REMARKETING quando aplicável) |
| VERSÃO | V01, V02, V03… |

A lista completa dos 29 nomes está em `../dados/nomes-criativos.csv`.

## 4. Arquivos

```
formato_conceito_angulo_versao_proporcao[_duracao].extensao
```

Exemplo: `reels_taxa-media_educativo_v01_9x16_15s.mp4`

Sem acentos, sem espaços, tudo em minúsculas, hífens dentro dos campos e sublinhados entre eles.

## 5. Regras

- Não renomear anúncios após a publicação.
- Uma nova versão altera `VERSÃO`; uma nova ideia altera `CONCEITO` ou `ÂNGULO`.
- Anúncios de remarketing usam `REMARKETING` no ângulo.
- Públicos de remarketing: `RMK | FONTE | JANELA`, por exemplo `RMK | VÍDEO 25% | 30D` (janelas a confirmar).
