# VendasOnline

Repositório canônico da operação pessoal de pesquisa de mercado, seleção de produtos, afiliados, dropshipping, e-commerce e futura automação da inteligência comercial.

## Objetivo atual

A fase atual não é construir um SaaS. O objetivo é operar um agente de inteligência comercial capaz de encontrar oportunidades de venda, validar demanda, comparar marketplaces, analisar comissões, estimar viabilidade econômica, sugerir canais de aquisição e documentar aprendizados.

O foco inicial foi refinado para:

> Encontrar gadgets, periféricos de computador e produtos gamer com maior potencial de ganho como afiliado, priorizando receita esperada e não apenas volume bruto de vendas.

Fluxo operacional atual:

1. Pesquisar 20 produtos candidatos.
2. Selecionar 5 para análise aprofundada.
3. Selecionar 3 produtos elegíveis para teste.
4. Validar comissão, conversão potencial, demanda, tendência, concorrência e compatibilidade com tráfego pago.
5. Registrar resultados e usar o histórico para orientar o desenvolvimento futuro da ferramenta.

## Expansão geográfica

1. São Paulo.
2. Brasil.
3. América Latina.
4. Internacional.

## Fontes e marketplaces prioritários

- Mercado Livre
- Shopee
- Amazon
- AliExpress
- TikTok Shop
- Google Ads / Keyword Planner
- Meta / Instagram como canal de aquisição e inteligência criativa

Outros canais serão adicionados conforme relevância e viabilidade de acesso aos dados.

## Princípio central

Mais vendido não significa melhor oportunidade.

A análise deve combinar preço, comissão, conversão potencial, demanda, crescimento, competição, custo de aquisição, restrições de mídia paga, logística, qualidade do produto e potencial criativo.

## Documentação

- docs/00-EXECUTIVE/PROJECT_VISION.md — visão e objetivo operacional.
- docs/01-AGENT/MASTER_AGENT_PROMPT.md — prompt mestre do agente.
- docs/02-METHODOLOGY/AFFILIATE_OPPORTUNITY_METHOD.md — metodologia de seleção.
- docs/02-METHODOLOGY/HYPPADO_BENCHMARK.md — benchmark do Hyppado e diferenciação.
- docs/03-RESEARCH/2026-10-02-SAO-PAULO-MARKET-SCAN.md — primeira varredura geral.
- docs/03-RESEARCH/2026-10-02-GADGETS-PC-GAMES-SCAN.md — varredura de gadgets, PC e games.
- docs/04-ROADMAP/OPERATIONAL_ROADMAP.md — evolução operacional.
- docs/05-PRODUCT/FUTURE_APP_PRODUCT_BRIEF.md — visão da futura ferramenta.
- docs/06-DECISIONS/DECISION_LOG.md — decisões canônicas.
- docs/07-COMPLIANCE/AFFILIATE_AND_ADS_RULES.md — regras e verificações de compliance.
- .agent/STATUS.md — estado atual.
- .agent/CURRENT_TASK.md — tarefa atual.
- .agent/NEXT_ACTION.md — próximo passo.
- .agent/CHANGELOG.md — mudanças documentais e operacionais.

## Regra de evidência

Todo dado deve ser classificado como um dos seguintes:

- OBSERVED — observado diretamente em fonte confiável.
- DERIVED — calculado a partir de dados observados.
- ESTIMATED — estimativa.
- INFERRED — inferência baseada em sinais.
- UNKNOWN — indisponível.
- NEEDS_VERIFICATION — precisa ser revalidado antes de uso operacional.

Nenhuma estimativa deve ser apresentada como fato.

## Segurança

Nunca armazenar neste repositório:

- chaves de API;
- tokens;
- senhas;
- cookies de sessão;
- credenciais de marketplaces;
- dados pessoais desnecessários.

Segredos deverão existir apenas em secret managers ou variáveis de ambiente protegidas.

## Estado

FASE 1 — OPERAÇÃO ASSISTIDA POR AGENTE.

O desenvolvimento do software ficará para depois de a metodologia ter sido exercitada em pesquisas e testes reais suficientes para revelar quais automações realmente geram valor.
