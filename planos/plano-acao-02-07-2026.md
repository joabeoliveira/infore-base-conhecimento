# 🎯 Plano de Ação — Infore 4.0

**Data:** 02 de Julho de 2026
**Responsável:** Joabe Oliveira
**Status:** 🔄 Em Andamento

---

## 🏆 Fases Concluídas

### ✅ Fase 0 — Levantamento (TUDO CONCLUÍDO! 🎉)

| ID | Tarefa | Status |
|---|---|---|
| 0.1 | Visita inicial de levantamento | ✅ Concluído |
| 0.2 | Elaborar e apresentar proposta | ✅ Concluído |
| 0.3 | Visita presencial de acompanhamento — fluxo de compras | ✅ Concluído |
| 0.4 | Consolidação pós-visita e documento de requisitos funcionais | ✅ Concluído |
| 0.5 | Base de conhecimento do projeto (GitHub + Obsidian) | ✅ Concluído |
| 0.6 | Acesso e-mails corporativos (Denilson) | ✅ Concluído |
| 0.7 | Tabelas de preços de fornecedores (Riquelm/Alexandre) | ✅ Concluído |

### ✅ Fase 1 — Infraestrutura (TUDO CONCLUÍDO! 🎉)

| ID | Tarefa | Status |
|---|---|---|
| 1.1 | Contratação e setup inicial da VPS | ✅ Concluído |
| 1.2 | Instalação do n8n e Redis na VPS | ✅ Concluído |
| 1.3 | Configuração do PostgreSQL | ✅ Concluído |
| 1.4 | Setup do Redis para cache de cotações e filas | ✅ Concluído |
| 1.5 | Configurar subdomínio oficial e DNS (infore.com.br) | ✅ Concluído |

---

## 🔴 Fase 2 — Motor de IA de Cotação (Prazo Macro: 45 dias)

### ✅ Concluídas na Fase 2

| ID | Tarefa | Status |
|---|---|---|
| 2.1 | Análise exploratória dos dados (1.530 transações + Pareto) | ✅ Concluído |
| 2.2 | Scraper SerperAPI — Mercado Livre | ✅ Concluído |
| 2.3 | Scraper SerperAPI — Amazon, Magalu, Shopee, Kalunga | ✅ Concluído |
| 2.9 | Radar de Oportunidades — MVP web (React + Supabase + n8n + Serper) | ✅ Concluído |
| 2.10 | 3 workflows n8n de coleta de produtos | ✅ Concluído |
| 2.17 | Atualizar categorias/filtros do Radar (Material Informática, Boa Dica) | ✅ Concluído |

### 🔄 Em Andamento

#### 2.4 — Pipeline de OCR para PDFs de propostas

| Campo | Valor |
|---|---|
| **Prazo** | 07/07/2026 |
| **Responsável** | Joabe Oliveira |
| **Status** | 🔄 Em Andamento |

**Checklist:**
- [ ] Configurar `pytesseract` + `pypdf2` no ambiente
- [ ] Testar com 3 PDFs reais de propostas
- [ ] Extrair: fornecedor, itens, quantidades, preços unitários/totais
- [ ] Estruturar saída em JSON padronizado

---

#### 2.5 — Motor de comparação inteligente via LLM

| Campo | Valor |
|---|---|
| **Prazo** | 28/07/2026 |
| **Responsável** | Joabe Oliveira |
| **Status** | 🔄 Em Andamento |

**Checklist:**
- [ ] Definir qual LLM usar (DeepSeek, Claude, GPT-4o)
- [ ] Criar prompt de comparação de preços
- [ ] Testar com dados dos 10 produtos do Pareto
- [ ] Validar acurácia com a equipe Infore

---

#### 2.13 — Pipeline de e-mails corporativos (Apps Script + motor de busca)

| Campo | Valor |
|---|---|
| **Prazo** | 30/07/2026 |
| **Responsável** | Joabe Oliveira |
| **Status** | 🔄 Em Andamento |
| **Nota** | Acessos já liberados (0.6 ✅) |

**Checklist:**
- [ ] Configurar Apps Script para ler e-mails de fornecedores
- [ ] Integrar resultado ao motor de busca SerperAPI
- [ ] Conectar ao fluxo de cotação

---

#### 2.14 — Integração Bitrix com motor de busca e fluxo de orçamentos

| Campo | Valor |
|---|---|
| **Prazo** | 05/08/2026 |
| **Responsável** | Joabe Oliveira |
| **Status** | 🔄 Em Andamento |

**Checklist:**
- [ ] Mapear endpoints de orçamentos no Bitrix
- [ ] Conectar motor de busca ao Bitrix
- [ ] Criar fluxo de orçamento automatizado

---

#### 2.15 — Catálogo interno com markup automático (30-40%)

| Campo | Valor |
|---|---|
| **Prazo** | 05/08/2026 |
| **Responsável** | Joabe Oliveira |
| **Status** | 🔄 Em Andamento |

**Checklist:**
- [ ] Definir regras de markup por categoria
- [ ] Integrar com tabelas de fornecedores (0.7 ✅)
- [ ] Automatizar atualização de preços

---

#### 2.16 — Links de afiliado (ML, Amazon, Shopee, Magalu)

| Campo | Valor |
|---|---|
| **Prazo** | 30/07/2026 |
| **Responsável** | Joabe + Riquelm |
| **Status** | 🔄 Em Andamento |

**Checklist:**
- [ ] Alinhar com Riquelm quais contas estão ativas
- [ ] Integrar links ao Radar de Oportunidades
- [ ] Validar markup de afiliado sendo contabilizado

**Contexto:** ~R$ 25K perdidos em 5 meses sem links de afiliado.

---

#### 2.19 — Ampliar fontes do Radar (Kalunga, Boa Dica, Americanas)

| Campo | Valor |
|---|---|
| **Prazo** | 25/07/2026 |
| **Responsável** | Joabe Oliveira |
| **Status** | 🔄 Em Andamento |

**Checklist:**
- [ ] Criar workflow/script SerperAPI para Kalunga
- [ ] Criar workflow/script SerperAPI para Boa Dica
- [ ] Criar workflow/script SerperAPI para Americanas
- [ ] Adicionar como fontes selecionáveis no Radar
- [ ] Testar com 5 produtos reais

---

### ⚪ Pendentes

#### 2.6 — Sistema de recomendação de menor preço com margem

| Prazo | Status |
|---|---|
| 05/07/2026 | ⚪ Pendente |

**Ações:**
- Aproveitar output do motor LLM (2.5)
- Adicionar cálculo de markup automático (30-40%)
- Gerar ranking final de fornecedores

---

#### 2.7 — Integração n8n — fluxo completo de cotação

| Prazo | Status |
|---|---|
| 12/07/2026 | ⚪ Pendente |

**Ações:**
- Conectar: pedido → busca → compara → sugere
- Orquestrar todos os scrapers + LLM + markup

---

#### 2.8 — Testes com dados reais (10 produtos do Pareto)

| Prazo | Status |
|---|---|
| 17/07/2026 | ⚪ Pendente |

**Ações:**
- Rodar motor completo contra Headset H390 e outros 9
- Validar resultados com equipe Infore

---

#### 2.12 — Cotação rápida com IA (supervisão humana)

| Prazo | Status |
|---|---|
| 25/07/2026 | ⚪ Pendente |

**Checklist:**
1. Pegar os 10 produtos do Pareto
2. Rodar pelo Radar + SerperAPI para coletar preços
3. Definir formato de saída ideal
4. Validar markup (30-40%) com dados reais
5. Apresentar para aprovação da equipe Infore
6. Automatizar fluxo no n8n

---

#### 2.18 — Documentar lojas de confiança para Compras Paraguai

| Prazo | Status |
|---|---|
| 30/07/2026 | ⚪ Pendente |

**Checklist:**
- [ ] Solicitar lista ao Riquelm
- [ ] Documentar em markdown na base de conhecimento
- [ ] Associar categorias de produtos a cada loja

---

#### 2.20 — Mapear itens do catálogo sem preço e automatizar

| Prazo | Status |
|---|---|
| 28/07/2026 | ⚪ Pendente |

**Checklist:**
- [ ] Exportar catálogo do Bitrix/CPLUS para planilha
- [ ] Filtrar itens com preço vazio
- [ ] Buscar no Radar automaticamente para cada SKU
- [ ] Alimentar planilha com preços + markup
- [ ] Programar atualização periódica

---

## ⚪ Fase 3 — Portal Next.js (Prazo Macro: 40 dias)

| ID | Tarefa | Prazo | Status |
|---|---|---|---|
| 3.1 | Desenvolvimento interface Next.js (login, dashboard, cotações) | 05/08/2026 | ⚪ Pendente |
| 3.2 | Dashboard de análise de preços e histórico | 12/08/2026 | ⚪ Pendente |
| 3.3 | Interface de solicitação de cotação (cliente interno) | 18/08/2026 | ⚪ Pendente |
| 3.4 | Integração do portal com motor de IA e n8n | 27/08/2026 | ⚪ Pendente |
| 3.5 | Interface do catálogo externo para clientes | 15/07/2026 | ⚪ Pendente |

---

## ⚪ Fase 4 — Integração CPLUS 5 (Prazo Macro: 20 dias)

| ID | Tarefa | Prazo | Status |
|---|---|---|---|
| 4.1 | Aguardar retorno VVS (auth, sandbox, webhooks) | 04/09/2026 | ⚪ Pendente |
| 4.2 | Implementar integração API CPLUS 5 (Orçamentos e Vendas) | 15/09/2026 | ⚪ Pendente |
| 4.3 | Fluxo automático cotação IA → orçamento CPLUS | 20/09/2026 | ⚪ Pendente |

---

## ⚪ Fase 5 — Capacitação (Prazo Macro: 30 dias)

| ID | Tarefa | Prazo | Status |
|---|---|---|---|
| 5.1 | Elaboração do Manual de Operação | 01/10/2026 | ⚪ Pendente |
| 5.2 | Preparação do material didático (Workshop de IAs) | 11/10/2026 | ⚪ Pendente |
| 5.3 | Treinamento da equipe (ChatGPT, Gemini e rotinas) | 25/10/2026 | ⚪ Pendente |

---

## 🔥 PRÓXIMOS PASSOS (Julho 2026)

**Top 3 prioridades para esta semana (02 a 05/07):**

1. **🖨️ 2.4 — OCR de PDFs** (vence 07/07) — configurar pytesseract + pypdf2, testar com 3 PDFs reais
2. **🧠 2.5 — Motor LLM** (vence 28/07) — definir modelo, criar prompt de comparação
3. **📡 2.19 — Ampliar Radar** (vence 25/07) — scripts SerperAPI para Kalunga, Boa Dica, Americanas

**Próxima semana (06 a 12/07):**
4. **🔄 2.7 — Integração n8n** — fluxo completo pedido → busca → compara → sugere
5. **📊 2.6 — Recomendação menor preço** — ranking final de fornecedores

---

## 📊 Visão Geral do Cronograma

### Total: 42 tarefas

| Status | Quantidade | % |
|---|---|---|
| ✅ Concluído | 18 | 43% |
| 🔄 Em Andamento | 7 | 17% |
| ⚪ Pendente | 17 | 40% |

### Progresso por Fase

| Fase | Concluídas | Andamento | Pendentes | Total |
|---|---|---|---|---|
| **Fase 0** — Levantamento | 7 | — | — | **7 ✅** |
| **Fase 1** — Infraestrutura | 5 | — | — | **5 ✅** |
| **Fase 2** — Motor IA Cotação | 6 | 7 | 6 | **19** |
| **Fase 3** — Portal Next.js | — | — | 5 | **5** |
| **Fase 4** — Integração CPLUS | — | — | 3 | **3** |
| **Fase 5** — Capacitação | — | — | 3 | **3** |

### Marcos Alcançados 🏆

- ✅ **Fase 0 completa** — Levantamento finalizado
- ✅ **Fase 1 completa** — Infraestrutura pronta (VPS, n8n, Redis, PostgreSQL, DNS)
- ✅ **Radar de Oportunidades no ar** → oportunidades.infore.cloud
- ✅ **3 workflows n8n de coleta** rodando
- ✅ **Acessos e e-mails liberados** (Denilson)
- ✅ **Tabelas de fornecedores recebidas** (Riquelm/Alexandre)

---

> 📝 **Última atualização:** 02/07/2026
> 📍 **Repositório:** [github.com/joabeoliveira/infore-base-conhecimento](https://github.com/joabeoliveira/infore-base-conhecimento)
> 📊 **Planilha oficial:** [Cronograma Infore 4.0](https://docs.google.com/spreadsheets/d/1gN1EKpSKMVEAf65D7pRZOhwL8m-6hro0ELiZNpA8zy8/edit)
