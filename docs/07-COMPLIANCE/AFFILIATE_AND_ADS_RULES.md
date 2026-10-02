# Compliance — Afiliados e Aquisição

Data-base inicial: 2026-10-02.

## Objetivo

Evitar recomendar uma combinação Produto + Programa + Canal que viole regras do marketplace, do afiliado ou da plataforma de anúncios.

Regras mudam. Sempre revalidar antes de investir.

## Mercado Livre

Fontes oficiais:

- https://www.mercadolivre.com.br/l/afiliados-ganhos-por-venda
- https://www.mercadolivre.com.br/l/afiliados-midia-paga
- https://www.mercadolivre.com.br/l/primeiros-passos-perguntas-frequentes-para-afiliados

Snapshot operacional:

- mídias sociais podem ser elegíveis conforme regras vigentes;
- Search/Shopping direcionando links afiliados não deve ser presumido como permitido;
- comissão depende de categoria e regras atuais.

Estado:

REVALIDATE_BEFORE_CAMPAIGN.

## Shopee

Fontes oficiais:

- https://help.shopee.com.br/portal/10/article/124094-Programa-de-Afiliados-da-Shopee-Termos-e-Condi%C3%A7%C3%B5es
- https://help.shopee.com.br/portal/10/article/128461-Como-gerar-seus-links-de-Afiliado-ou-ID-de-produto-para-compartilhar
- https://help.shopee.com.br/portal/10/article/223989-Atualiza%C3%A7%C3%A3o%20na%20Comiss%C3%A3o%20de%20Shopee%20Video

Snapshot operacional:

- analisar canais sociais permitidos;
- considerar Comissão Extra;
- não presumir elegibilidade de Google Search/Shopping para links afiliados.

Estado:

REVALIDATE_BEFORE_CAMPAIGN.

## Amazon Associados

Fontes:

- https://associados.amazon.com.br/help/node/topic/GRXPHT8U84RAYDXZ
- https://associados.amazon.com.br/help/operating/compare

Snapshot operacional:

- tabela de remuneração varia conforme categoria/formato;
- mudanças de 2026 tornaram publicidade paga vinculada à Amazon um ponto de atenção;
- não executar campanha paga baseada em comissão sem ler a regra vigente.

Estado:

REVIEW_REQUIRED.

## TikTok Shop

Fontes:

- https://seller-br.tiktok.com/university/essay?knowledge_id=3355295847515925
- https://seller-br.tiktok.com/university/essay?knowledge_id=1517752301717265

Snapshot:

- comissão varia por categoria;
- sellers podem configurar oportunidades de comissão;
- pesquisar oferta por produto é essencial.

Estado:

PRODUCT_LEVEL_REVIEW.

## AliExpress

Estado atual:

NEEDS_VERIFICATION.

A operação não deve assumir percentual genérico nem canal permitido sem documentação vigente da conta/região.

## Anatel

Fonte:

https://www.gov.br/anatel/pt-br/regulado/certificacao-de-produtos/duvidas-frequentes

Produtos com radiofrequência, incluindo diversas categorias Bluetooth/Wi-Fi, podem estar sujeitos a homologação aplicável para comercialização no Brasil.

Estado:

REGULATORY_REVIEW_REQUIRED para produtos wireless destinados a operação própria/importação.

## Matriz conceitual

Toda oportunidade deverá ter:

- marketplace;
- programa;
- país;
- canal;
- policy_source;
- verified_at;
- status;
- restriction;
- notes.

Estados:

- ALLOWED
- ALLOWED_WITH_RESTRICTIONS
- UNKNOWN
- REVIEW_REQUIRED
- PROHIBITED

## Regra operacional

Compliance nunca deve ser inferido apenas porque outra pessoa anuncia o produto.

A fonte de decisão deve ser regra oficial vigente.
