# Criar diretório e todos os arquivos da wiki
mkdir -p /tmp/infore-kb

cat > /tmp/infore-kb/infore.md << 'KBEOF'
---
title: Infore
created: 2026-06-02
updated: 2026-06-02
type: entity
tags: [empresa, hub-suprimentos, logistica, infraestrutura, rio-de-janeiro, b2b]
sources: [raw/articles/infore-home.md]
confidence: medium
---

# Infore

## Visão Geral
A **Infore** é um hub de [[suprimentos-corporativos]] B2B com sede em Campo Grande, Rio de Janeiro. Atua como centralizador de compras, [[logistica-regional]] e infraestrutura para empresas.

**Slogan:** "Seu principal Hub de suprimentos, logística e infraestrutura no Rio de Janeiro"

**Sede:** Estr. da Cachamorra, 3300 – Campo Grande, Rio de Janeiro – RJ
**Tempo de mercado:** 23+ anos
**Site:** https://infore.com.br
**Contato:** contato@infore.com.br | (21) 4040-3364

## Proposta de Valor
- **Centralização de compras** — um parceiro único substitui múltiplos fornecedores
- **[[atendimento-consultivo]]** — atendimento humano, sem robôs
- **[[logistica-regional]]** própria — entrega ágil em todo o RJ
- **[[estoque-just-in-time]]** — almoxarifado virtual dos clientes

> "Do alfinete ao foguete. A gente Entrega o que Ninguém Consegue!"

## Cobertura
Atende todas as regiões do RJ: Metropolitana, Norte, Noroeste, Serrana, Baixadas Litorâneas, Centro-Sul, Médio Vale do Paraíba, Costa Verde.

## Páginas Relacionadas
- [[suprimentos-corporativos]]
- [[logistica-regional]]
- [[atendimento-consultivo]]
- [[estoque-just-in-time]]
KBEOF

cat > /tmp/infore-kb/suprimentos-corporativos.md << 'KBEOF'
---
title: Suprimentos Corporativos
created: 2026-06-02
type: concept
tags: [suprimentos-corporativos, b2b, compras, supply-chain]
sources: [raw/articles/infore-home.md]
---

# Suprimentos Corporativos

Fornecimento de materiais e insumos para empresas (B2B). A [[infore]] opera como **hub centralizador**: em vez do cliente gerenciar dezenas de fornecedores, consolida toda a demanda em um único parceiro.

## Benefícios
- Redução de custos com múltiplos fornecedores e fretes
- Previsibilidade com SLAs definidos
- Menos overhead administrativo

## Relacionado
- [[estoque-just-in-time]]
- [[logistica-regional]]
- [[atendimento-consultivo]]
KBEOF

cat > /tmp/infore-kb/logistica-regional.md << 'KBEOF'
---
title: Logística Regional
created: 2026-06-02
type: concept
tags: [logistica, regional, rio-de-janeiro, dna-carioca]
sources: [raw/articles/infore-home.md]
---

# Logística Regional

Operação de transporte focada no Rio de Janeiro, com logística própria e conhecimento profundo do território. A [[infore]] usa isso como vantagem competitiva contra distribuidores nacionais.

## DNA Carioca
"Conhecemos a logística do Rio de Janeiro. Entregamos na Zona Sul, Zona Norte, Zona Oeste e em todo o estado — sem as desculpas dos grandes centros nacionais."

## Cobertura
Todas as regiões do RJ com SLA e padrão profissional.

## Relacionado
- [[estoque-just-in-time]]
- [[suprimentos-corporativos]]
- [[infore]]
KBEOF

cat > /tmp/infore-kb/atendimento-consultivo.md << 'KBEOF'
---
title: Atendimento Consultivo
created: 2026-06-02
type: concept
tags: [atendimento-consultivo, b2b, diferencial]
sources: [raw/articles/infore-home.md]
---

# Atendimento Consultivo

Modelo onde o fornecedor atua como **consultor de compras**, não só tomador de pedidos. A [[infore]] usa isso como diferencial: "Você não fala com robô nem fica perdido em atendimento genérico."

## Características
- **Humano** — sem chatbots ou call center genérico
- **Próximo** — equipe conhece o cliente
- **Ágil** — resolução rápida
- **Consultivo** — evita compras erradas, otimiza orçamento

## Relacionado
- [[suprimentos-corporativos]]
- [[infore]]
- [[logistica-regional]]
KBEOF

cat > /tmp/infore-kb/estoque-just-in-time.md << 'KBEOF'
---
title: Estoque Just-in-Time
created: 2026-06-02
type: concept
tags: [just-in-time, almoxarifado-virtual, supply-chain]
sources: [raw/articles/infore-home.md]
---

# Estoque Just-in-Time

