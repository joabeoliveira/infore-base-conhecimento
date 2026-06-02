---
title: Fornecedores, Ranking e Relacionamento
created: 2026-06-02
updated: 2026-06-02
type: process
tags: [fornecedores, ranking, relacionamento, performance, rentabilidade]
sources: [PLANO_AJUSTES_MVP.md, visita-relatorios/dia-28-05-26/lista-maior-para-o-menor-fornecedores-por-quantidade-compras.csv, visita-relatorios/dia-28-05-26/lista-fornecedores-lucrativo.csv]
confidence: high
---

# Fornecedores, Ranking e Relacionamento

## Definicao e objetivo
Este no organiza criterios de avaliacao de fornecedores para apoiar decisoes de compra com consistencia. O objetivo e equilibrar preco, confiabilidade e resultado de margem para a [[infore]].

## Contexto operacional Infore
A operacao combina marketplaces e fornecedores especializados. No dia a dia, o historico real de compras e importante para reduzir risco em [[cotacao-preco-arbitragem]] e aumentar previsibilidade em [[fluxo-pedidos-vendedor-comprador]].

## Criterios de ranking
- Recorrencia de compras e historico de atendimento
- Competitividade de preco por categoria
- Qualidade do item entregue em relacao ao solicitado
- Prazo real de entrega e estabilidade operacional
- Resultado de margem observado nas vendas

## Regras de decisao
- Em empate tecnico e comercial, priorizar fornecedor com melhor historico.
- Fornecedor com recorrencia de falhas deve ter prioridade reduzida.
- Fornecedor especialista pode ser preferido em categorias criticas.
- O menor preco nao prevalece quando houver risco alto de especificacao incorreta.

## Relacionamento e estrategia
- Manter carteira principal por categoria para reduzir variancia.
- Revisar ranking periodicamente com base em dados recentes.
- Tratar fornecedores de oportunidade como complemento, nao base unica.

## Casos-limite e excecoes
- Novo fornecedor sem historico: usar em escala controlada.
- Alta urgencia com baixa oferta: selecionar melhor opcao disponivel e registrar excecao.
- Categoria com grande dispersao de qualidade: aumentar peso de confiabilidade.

## Sinais praticos para uso do Hermes
- O Hermes deve indicar quando a recomendacao contraria o ranking historico e explicar o motivo.
- O Hermes deve explicitar risco de fornecedor novo ou sem amostra suficiente.
- O Hermes deve sugerir revisao humana quando houver conflito entre margem e confiabilidade.

## Paginas relacionadas
- [[infore]]
- [[suprimentos-corporativos]]
- [[cotacao-preco-arbitragem]]
- [[precificacao-markup-margem]]
- [[analytics-rentabilidade-fornecedor-margem]]
- [[fluxo-pedidos-vendedor-comprador]]
- [[operacao-paraguai-especialista]]
- [[abastecimento-demanda-sourcing-heterogeneo]]
- [[logistica-regional]]
- [[hermes-agent]]
