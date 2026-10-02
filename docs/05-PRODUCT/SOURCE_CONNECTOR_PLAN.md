# Plano de Fontes e Conectores

## Objetivo

Projetar a futura coleta sem acoplar a operação a uma única plataforma.

## Prioridade 1

### Mercado Livre

Usos pretendidos:

- catálogo;
- tendências quando disponíveis;
- rankings/highlights;
- preço;
- seller;
- categoria;
- programa de afiliados.

Referência de tendências:

https://developers.mercadolivre.com.br/en_us/trends

Estado:

HIGH_PRIORITY.

### Google Ads / Keyword Planner

Usos pretendidos:

- volume de pesquisa;
- concorrência;
- CPC;
- geo targeting;
- demanda regional.

Referências:

https://developers.google.com/google-ads/api/docs/keyword-planning/overview

https://developers.google.com/google-ads/api/docs/keyword-planning/generate-historical-metrics

Estado:

HIGH_PRIORITY para enriquecer São Paulo.

## Prioridade 2

### Shopee

Usos:

- catálogo;
- preço;
- seller;
- afiliado;
- Comissão Extra;
- sinais de venda quando expostos.

Estado:

FEASIBILITY_REVIEW_REQUIRED.

### Amazon

Usos:

- catálogo;
- preço;
- afiliado;
- categorias;
- comparação de oferta.

Estado:

FEASIBILITY_REVIEW_REQUIRED.

### TikTok Shop

Usos:

- social commerce;
- comissão;
- produtos;
- criativos/tendências conforme acesso permitido.

Estado:

HIGH_VALUE / ACCESS_DEPENDENT.

### AliExpress

Usos:

- sourcing;
- preço;
- catálogo;
- afiliado.

Estado:

NEEDS_VERIFICATION.

## Regra arquitetural

Cada integração futura deve expor um contrato normalizado.

Exemplo conceitual:

Provider
- searchProducts()
- getProduct()
- getOffers()
- getAffiliateTerms()
- getTrendSignals()
- getSellerSignals()

Nem todo provider implementará todos os métodos.

Usar capability flags para declarar suporte.

## Rate Limits e resiliência

Planejar:

- retries;
- exponential backoff;
- rate limiting;
- cache;
- dead letter;
- idempotência;
- observabilidade;
- quota monitoring.

Uma fonte indisponível não pode derrubar todo o sistema.

## Proibição

Não tratar scraping proibido por termos como solução padrão para ausência de API.
