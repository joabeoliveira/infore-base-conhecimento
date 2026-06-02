---
title: Operacao Paraguai e Dependencia de Especialista
created: 2026-06-02
updated: 2026-06-02
type: process
tags: [paraguai, importacao, negociacao, risco-operacional, especialista]
sources: [visita-relatorios/dia-28-05-26/05-28 Compra no Paraguai_ Fluxo Manual, Dependencia de Especialista e Riscos Operacionais-Summary.md, PLANO_AJUSTES_MVP.md]
confidence: high
---

# Operacao Paraguai e Dependencia de Especialista

## Definicao e objetivo
Este no descreve o fluxo de compra no Paraguai e seus pontos criticos de decisao. O objetivo e reduzir risco de dependencia de pessoa unica e tornar a operacao reproduzivel no contexto da [[infore]].

## Contexto operacional Infore
A operacao PY acontece fora do fluxo padrao e envolve validacoes adicionais de preco, produto, cambio e retirada. Historicamente, a execucao concentra conhecimento em especialista, o que aumenta risco de continuidade.

## Etapas principais
- Identificacao de oportunidade de compra no Paraguai durante a cotacao
- Validacao final de aderencia tecnica e vantagem economica
- Negociacao com loja e confirmacao de condicoes
- Pagamento via parceiro de cambio
- Liberacao, retirada e transporte para entrega

## Regras de decisao
- So considerar PY quando houver ganho economico relevante versus compra local.
- Validar especificacao de produto com rigor para evitar erro de item similar.
- Registrar justificativa de escolha PY no pedido para rastreabilidade.
- Em ausencia de especialista disponivel, escalar para revisao humana com checklist obrigatorio.

## Casos-limite e excecoes
- Diferenca de preco pequena: priorizar compra local por simplicidade operacional.
- Produto de alto risco tecnico: exigir dupla validacao antes de fechar.
- Falha de parceiro logistico/cambio: acionar plano alternativo e reavaliar viabilidade.

## Sinais praticos para uso do Hermes
- O Hermes deve sinalizar quando a recomendacao PY depende de premissa fraca.
- O Hermes deve separar ganho de preco de risco operacional total.
- O Hermes deve sugerir revisao humana quando a operacao envolver muitos intermediarios.

## Paginas relacionadas
- [[infore]]
- [[cotacao-preco-arbitragem]]
- [[fornecedores-ranking-relacionamento]]
- [[fluxo-pedidos-vendedor-comprador]]
- [[precificacao-markup-margem]]
- [[hermes-agent]]
