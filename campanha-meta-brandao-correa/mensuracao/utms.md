# UTMs e eventos

## 1. Modelo de UTMs

```
utm_source=meta
utm_medium=paid_social
utm_campaign=leads_financiamento_veiculos
utm_content={{ad.name}}
utm_term={{adset.name}}
```

- `utm_campaign`: nome da campanha, fixo.
- `utm_content`: nome do **anúncio** (parâmetro dinâmico `{{ad.name}}`).
- `utm_term`: nome do **conjunto** (parâmetro dinâmico `{{adset.name}}`).

Os nomes seguem `nomes-padroes.md`. Eles contêm espaços, acentos e barras; os parâmetros dinâmicos da Meta substituem o valor e codificam a URL, mas **teste o link no rastreamento do site antes de publicar** (a confirmar).

### Exemplo de URL final

```
https://brandaocorrea.bitrix24.site/2684/?utm_source=meta&utm_medium=paid_social&utm_campaign=leads_financiamento_veiculos&utm_content={{ad.name}}&utm_term={{adset.name}}
```

Para identificar a campanha, o conjunto e o anúncio pelos IDs também, considerar adicionar `{{campaign.id}}`, `{{adset.id}}`, `{{ad.id}}` como parâmetros extras (a confirmar).

## 2. Limitação importante dos formulários nativos

**[Provável]** UTMs só viajam quando a pessoa **clica para um site**. Quem preenche o formulário dentro da plataforma não passa pela URL. O lead chega com os identificadores do próprio formulário (campanha, conjunto, anúncio e formulário), disponíveis pela integração de leads ou pelo download de leads (a confirmar).

Consequência prática: no Bitrix24, registrar a **origem do lead** a partir dos campos do formulário (ID/nome do anúncio, do conjunto e da campanha) e, quando a pessoa chegar pela landing page, a partir das UTMs. Sem isso, não será possível medir custo por lead qualificado por criativo.

## 3. Eventos recomendados

| Evento | Onde | Observação |
|---|---|---|
| `Lead` | Formulário nativo e landing page | Evento principal |
| `PageView` | Landing page | Exige pixel instalado (a confirmar em `bitrix24.site`) |
| `ViewContent` | Landing page | Leitura do conteúdo |
| `Contact` ou personalizado | Clique em atendimento (se houver botão de WhatsApp) | A confirmar |
| `LeadQualificado` (personalizado) | CRM → Meta | Envio a partir do Bitrix24 após a triagem. Exige configuração de API de conversões, **fora do escopo deste pacote** |
| `AtendimentoIniciado` (personalizado) | CRM → Meta | Idem |

## 4. Mensuração por criativo

Cada criativo tem nome único (`nomes-padroes.md`). O nome do anúncio é a chave para ligar o lead ao criativo. Não renomear anúncios depois de publicados.
