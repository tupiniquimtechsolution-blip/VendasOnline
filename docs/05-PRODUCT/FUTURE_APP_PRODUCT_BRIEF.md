# Product Brief — Futura Ferramenta VendasOnline

## Estado

PLANEJAMENTO FUTURO.

Não iniciar desenvolvimento amplo ainda.

## Visão

Transformar a metodologia validada pelo agente em uma plataforma pessoal de Market Intelligence, Product Intelligence e Affiliate/Commerce Intelligence.

## Pergunta que a ferramenta deverá responder

> Qual produto vale investigar ou testar, em qual mercado, em qual marketplace, com qual comissão/margem, usando qual canal, com quais riscos e baseado em quais evidências?

## Diferencial

Não ser apenas uma lista de produtos virais.

Cruzar:

- marketplace;
- região;
- nicho;
- produto;
- demanda;
- tendência;
- preço;
- comissão;
- concorrência;
- tráfego pago;
- conteúdo;
- logística;
- compliance;
- resultados reais.

## Filtros planejados

### Geografia

- país;
- estado/região;
- cidade quando suportado;
- região postal quando suportado.

### Marketplace

- Mercado Livre;
- Shopee;
- Amazon;
- AliExpress;
- TikTok Shop;
- extensível para outros.

### Produto

- categoria;
- subcategoria;
- preço;
- ticket;
- avaliações;
- rating;
- vendas/proxies;
- crescimento;
- seller count;
- comissão;
- CRPS;
- EAR;
- Opportunity Score.

### Operação

- afiliado;
- dropshipping nacional;
- dropshipping internacional;
- estoque próprio;
- seller;
- loja própria.

### Aquisição

- Meta Ads;
- Instagram;
- TikTok;
- Google Ads;
- Shopping;
- orgânico.

## Arquitetura conceitual

External Sources
-> Source Adapters
-> Collection Jobs
-> Raw Storage
-> Normalization
-> Product Matching
-> Enrichment
-> Analytics
-> Opportunity Engine
-> Application API
-> Web UI

## Source Adapters

Planejar adaptadores isolados:

- MercadoLivreAdapter
- ShopeeAdapter
- AmazonAdapter
- AliExpressAdapter
- TikTokShopAdapter
- GoogleAdsAdapter
- MetaSignalsAdapter

A lógica específica de um provider não deve contaminar o domínio central.

## Modelo de dados conceitual

Entidades candidatas:

- Geography
- Marketplace
- CanonicalProduct
- MarketplaceListing
- Seller
- Offer
- PriceSnapshot
- DemandSnapshot
- KeywordSnapshot
- AdvertisingSignal
- AffiliateProgram
- AffiliateOffer
- ComplianceRule
- OpportunitySnapshot
- Campaign
- Creative
- ResearchRun
- Decision

## Provenance

Todo dado deverá registrar, conforme aplicável:

- source;
- collected_at;
- geography;
- source_type;
- confidence;
- raw_value;
- normalized_value.

Classificações:

OBSERVED, DERIVED, ESTIMATED, INFERRED, UNKNOWN.

## Opportunity Engine

A futura versão deve utilizar pesos configuráveis e versionados.

Na fase afiliada, Affiliate Revenue Potential deve ter peso central.

Nunca hardcode de forma irreversível pesos de scoring.

## Product 360

Cada produto deverá reunir:

- listings;
- preços;
- histórico;
- marketplaces;
- comissão;
- ganho por venda;
- demanda;
- tendência;
- concorrência;
- políticas;
- criativos;
- histórico de testes;
- score.

## Compliance Engine

Combinação:

Marketplace + Programa + País + Canal de Aquisição + Modelo Comercial

Estados sugeridos:

- ALLOWED
- ALLOWED_WITH_RESTRICTIONS
- UNKNOWN
- REVIEW_REQUIRED
- PROHIBITED

Armazenar:

- policy_source;
- policy_version;
- verified_at;
- restriction;
- evidence_url.

## Stack inicial a avaliar no futuro

Baseline, não decisão definitiva:

- Frontend: Next.js + TypeScript
- UI: Tailwind + componentes acessíveis
- Backend: TypeScript/NestJS ou alternativa justificada
- Workers/Analytics: Python quando necessário
- Database: PostgreSQL
- Cache/Queue: Redis / BullMQ ou equivalente
- Object Storage: S3-compatible

Não introduzir arquitetura distribuída sem necessidade real.

## MVP futuro

Somente após validação operacional.

Módulos prováveis:

1. Market Explorer
2. Product Explorer
3. Product 360
4. Affiliate Opportunity Score
5. Compliance Matrix
6. Watchlist
7. Marketing Lab
8. Research History

## Não objetivos iniciais

- virar marketplace;
- processar pagamentos;
- operar logística;
- ter milhões de usuários;
- suportar todos os países;
- criar dezenas de integrações antes de validar valor.

## Gate para desenvolvimento

O software começa quando houver evidência de que a automação economiza tempo ou melhora a qualidade das decisões comerciais.
