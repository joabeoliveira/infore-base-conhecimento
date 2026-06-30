# 🎯 Plano de Ação — Infore 4.0

**Data:** 30 de Junho de 2026
**Responsável:** Joabe Oliveira
**Status:** 🔄 Em Andamento

---

## Sumário

- [🔴 Onda 1 — Fogo (hoje e amanhã)](#onda-1--fogo-hoje-e-amanhã)
- [🟡 Onda 2 — Semana (01 a 05/07)](#onda-2--semana-01-a-0507)
- [⚪ Onda 3 — Próxima Semana (05 a 12/07)](#onda-3--próxima-semana-05-a-1207)
- [👥 Ações com Terceiros](#ações-com-terceiros)
- [📊 Visão Geral do Cronograma](#visão-geral-do-cronograma)

---

## 🔴 Onda 1 — Fogo (hoje e amanhã)

Tarefas vencidas e urgentes — impacto imediato.

### 2.13 — Pipeline de e-mails corporativos (Apps Script + motor de busca)

| Campo | Valor |
|---|---|
| **Prazo** | ~~30/06~~ 🚨 ATRASADA |
| **Responsável** | Joabe Oliveira |
| **Status** | 🔄 Em Andamento |
| **Dependência** | Tarefa 0.6 — Denilson liberar acessos |

**Checklist:**
- [ ] Confirmar com Denilson se os acessos já foram liberados
- [ ] Se sim: configurar script Apps Script para ler e-mails de fornecedores
- [ ] Se não: iniciar estrutura do motor de busca sem os e-mails (mock)
- [ ] Integrar resultado ao fluxo de cotação

---

### 2.16 — Links de afiliado (ML, Amazon, Shopee, Magalu)

| Campo | Valor |
|---|---|
| **Prazo** | ~~30/06~~ 🚨 ATRASADA |
| **Responsável** | Joabe + Riquelm |
| **Status** | 🔄 Em Andamento |

**Checklist:**
- [ ] Alinhar com Riquelm em reunião rápida (15 min)
- [ ] Confirmar quais contas de afiliado já estão ativas
- [ ] Integrar links ao Radar de Oportunidades
- [ ] Validar se o markup de afiliado está sendo contabilizado

**Contexto:** Estima-se ~R$ 25K perdidos em 5 meses sem links de afiliado.

---

### 2.12 — Cotação rápida IA com supervisão humana

| Campo | Valor |
|---|---|
| **Prazo** | ~~25/06~~ 🚨 ATRASADA |
| **Responsável** | Joabe Oliveira |
| **Status** | 🔴 Atrasado |

**Checklist:**

1. **Pegar os 10 produtos do Pareto** (ex: Headset H390, etc.)
2. **Rodar manualmente** pelo Radar + SerperAPI para coletar preços
3. **Definir o formato de saída** ideal (o que o comprador precisa ver)
4. **Validar markup** (30-40%) com base nos dados reais
5. **Apresentar para aprovação** da equipe Infore
6. **Automatizar o fluxo** no n8n

---

## 🟡 Onda 2 — Semana (01 a 05/07)

Tarefas que desbloqueiam entregas seguintes.

### 2.19 — Ampliar fontes do Radar (Kalunga, Boa Dica, Americanas)

| Campo | Valor |
|---|---|
| **Prazo** | ~~25/06~~ 🚨 ATRASADA |
| **Responsável** | Joabe Oliveira |
| **Status** | 🔴 Atrasado |

**Checklist:**
- [ ] Criar workflow n8n para Kalunga (ou script SerperAPI)
- [ ] Criar workflow n8n para Boa Dica
- [ ] Criar workflow n8n para Americanas
- [ ] Adicionar como fontes selecionáveis no Radar
- [ ] Testar com 5 produtos reais

**Observação:** É uma tarefa de ~2 horas por marketplace. SerperAPI cobre a maioria.

---

### 2.20 — Mapear itens do catálogo sem preço e automatizar

| Campo | Valor |
|---|---|
| **Prazo** | ~~28/06~~ 🚨 ATRASADA |
| **Responsável** | Joabe Oliveira |
| **Status** | 🔴 Atrasado |

**Checklist:**
- [ ] Exportar catálogo do Bitrix/CPLUS para planilha
- [ ] Filtrar itens com coluna de preço vazia
- [ ] Para cada SKU sem preço, buscar no Radar automaticamente
- [ ] Alimentar planilha com preços encontrados + markup
- [ ] Programar atualização periódica

---

### 1.5 — Configurar subdomínio oficial e DNS (infore.com.br)

| Campo | Valor |
|---|---|
| **Prazo** | ~~25/06~~ 🚨 ATRASADA |
| **Responsável** | Joabe Oliveira |
| **Status** | 🔴 Atrasado |

**Opções:**
- **Opção A (rápida):** Usar subdomínio temporário `plataforma.infore.cloud` via Hostinger — resolve em minutos
- **Opção B (oficial):** Solicitar registro `plataforma.infore.com.br` junto à Infore

**Checklist:**
- [ ] Decidir entre opção A ou B
- [ ] Se A: configurar DNS no Hostinger
- [ ] Se B: abrir chamado com a Infore para registro.br
- [ ] Configurar SSL (Let's Encrypt)

---

### 2.18 — Documentar lojas de confiança para Compras Paraguai

| Campo | Valor |
|---|---|
| **Prazo** | ~~30/06~~ 🚨 ATRASADA |
| **Responsável** | Joabe + Riquelm |
| **Status** | ⚪ Pendente |

**Checklist:**
- [ ] Solicitar lista ao Riquelm
- [ ] Documentar em markdown na base de conhecimento
- [ ] Associar categorias de produtos a cada loja

---

## ⚪ Onda 3 — Próxima Semana (05 a 12/07)

Tarefas pendentes que exigem preparação.

### 2.6 — Sistema de recomendação de menor preço com margem

| Prazo | Status |
|---|---|
| 05/07 | ⚪ Pendente |

**Ações:**
- Aproveitar output do motor LLM (tarefa 2.5)
- Adicionar cálculo de markup automático (30-40%)
- Gerar ranking final de fornecedores

### 2.15 — Catálogo interno com markup automático (30-40%)

| Prazo | Status |
|---|---|
| 05/07 | ⚪ Pendente |

**⚠️ Depende de:** Tarefa 0.7 (tabelas de fornecedores com Riquelm/Alexandre)

### 2.4 — Pipeline de OCR para PDFs de propostas

| Prazo | Status |
|---|---|
| 07/07 | 🔄 Em Andamento |

**Checklist:**
- [ ] Configurar `pytesseract` + `pypdf2` no ambiente
- [ ] Testar com 3 PDFs reais de propostas
- [ ] Extrair: fornecedor, itens, quantidades, preços unitários/totais
- [ ] Estruturar saída em JSON padronizado

### 2.5 — Motor de comparação inteligente via LLM

| Prazo | Status |
|---|---|
| 28/07 | 🔄 Em Andamento |

**Checklist:**
- [ ] Definir qual LLM usar (DeepSeek, Claude, GPT-4o)
- [ ] Criar prompt de comparação de preços
- [ ] Testar com dados dos 10 produtos do Pareto
- [ ] Validar acurácia com a equipe Infore

---

## 👥 Ações com Terceiros

| ID | Tarefa | Quem | O que cobrar | Status |
|---|---|---|---|---|
| 0.7 | Tabelas de fornecedores | **Riquelm / Alexandre** | Planilhas de custo atualizadas | 🔴 Pendente |
| 0.6 | Acesso e-mails corporativos | **Denilson** | Credenciais IMAP/SMTP + hospedagem | 🔄 Já solicitado |
| 2.18 | Compras Paraguai | **Riquelm** | Lista de lojas de confiança | ⚪ Pendente |
| 4.1 | Retorno API CPLUS 5 | **Iuri (VVS)** | 11 perguntas técnicas | ⏳ Aguardando |

---

## 📊 Visão Geral do Cronograma

### Total: 43 tarefas

| Status | Quantidade | % |
|---|---|---|
| ✅ Concluído | 20 | 46% |
| 🔄 Em Andamento | 8 | 19% |
| 🔴 Atrasado | 6 | 14% |
| ⚪ Pendente | 9 | 21% |

### Progresso por Fase

| Fase | Concluídas | Andamento | Atrasadas | Pendentes | Total |
|---|---|---|---|---|---|
| **Fase 0** — Levantamento | 4 | 1 (acessos) | — | 1 (tabelas) | 6 |
| **Fase 1** — Infraestrutura | 4 | — | 1 (DNS) | — | 5 |
| **Fase 2** — Motor IA Cotação | 6 | 5 | 4 | 4 | 19 |
| **Fase 3** — Portal Next.js | — | — | — | 5 | 5 |
| **Fase 4** — Integração CPLUS 5 | — | — | — | 3 | 3 |
| **Fase 5** — Capacitação | — | — | — | 3 | 3 |
| **Fase 2** (Radar/afiliados extras) | 2 | 2 | 1 | 2 | 7 |

---

> 📝 **Última atualização:** 30/06/2026
> 📍 **Repositório:** [github.com/joabeoliveira/infore-base-conhecimento](https://github.com/joabeoliveira/infore-base-conhecimento)
> 📊 **Planilha oficial:** [Cronograma Infore 4.0](https://docs.google.com/spreadsheets/d/1gN1EKpSKMVEAf65D7pRZOhwL8m-6hro0ELiZNpA8zy8/edit)
