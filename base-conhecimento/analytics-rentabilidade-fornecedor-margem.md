---
title: Analytics de Rentabilidade por Fornecedor e Margem
created: 2026-06-02
updated: 2026-06-02
type: process
tags: [analytics, rentabilidade, margem, fornecedores, decisao]
sources: [visita-relatorios/dia-28-05-26/lista-fornecedores-lucrativo.csv, visita-relatorios/dia-28-05-26/lista-maior-para-o-menor-fornecedores-por-quantidade-compras.csv, PLANO_AJUSTES_MVP.md]
confidence: high
---

# Analytics de Rentabilidade por Fornecedor e Margem

## Definicao e objetivo
Este no organiza a leitura de desempenho economico da operacao por fornecedor para apoiar decisoes de compra e precificacao. O objetivo e equilibrar volume, margem e risco na [[infore]].

## Contexto operacional Infore
A operacao possui fornecedores com alto volume e outros com alta margem por pedido. Sem leitura analitica continua, o processo pode privilegiar apenas recorrencia ou apenas preco, prejudicando resultado final.

## Indicadores-chave
- Volume de compras por fornecedor
- Lucro acumulado por fornecedor
- Margem estimada por categoria e canal
- Frequencia de uso com resultado positivo
- Variacao de desempenho ao longo do tempo

## Regras de decisao
- Nao decidir fornecedor apenas por volume historico.
- Nao decidir fornecedor apenas por lucro absoluto isolado.
- Combinar ranking operacional com desempenho de margem por contexto.
- Revisar estrategia quando houver queda recorrente de margem em fornecedor frequente.

## Leituras praticas com base no historico
- Fornecedor de alto volume tende a melhorar previsibilidade e velocidade.
- Fornecedor de alta margem tende a capturar oportunidades especificas.
- O equilibrio entre escala e margem melhora robustez da carteira.
- Operacoes especiais (ex.: PY) exigem avaliacao conjunta de lucro e risco operacional.

## Casos-limite e excecoes
- Lucro alto com baixa recorrencia: validar se ha repetibilidade antes de priorizar.
- Volume alto com margem em queda: investigar erosao de preco ou custo logistico.
- Dado inconsistente entre fontes: revisar base antes de ajustar ranking.

## Sinais praticos para uso do Hermes
- O Hermes deve indicar quando a recomendacao contraria tendencia de margem historica.
- O Hermes deve separar ganho pontual de ganho estrutural.
- O Hermes deve sugerir revisao humana quando houver trade-off forte entre margem e confiabilidade.

## Paginas relacionadas
- [[infore]]
- [[fornecedores-ranking-relacionamento]]
- [[precificacao-markup-margem]]
- [[cotacao-preco-arbitragem]]
- [[fluxo-pedidos-vendedor-comprador]]
- [[operacao-paraguai-especialista]]
- [[hermes-agent]]
