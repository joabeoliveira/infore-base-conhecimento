---
title: Precificacao, Markup e Margem
created: 2026-06-02
updated: 2026-06-02
type: process
tags: [precificacao, markup, margem, rentabilidade, decisao]
sources: [PLANO_AJUSTES_MVP.md, visita-relatorios/dia-28-05-26/lista-fornecedores-lucrativo.csv]
confidence: high
---

# Precificacao, Markup e Margem

## Definicao e objetivo
Precificacao e o processo de formar o preco de venda a partir do custo total, aplicando regras de markup e margem. O objetivo na [[infore]] e proteger rentabilidade sem perder competitividade.

## Contexto operacional Infore
A operacao comercial nao trabalha com preco de custo puro. O valor final depende de markup, frete e risco da operacao. Essa camada fecha o ciclo iniciado em [[intake-produto-especificacao-estruturada]] e [[cotacao-preco-arbitragem]].

## Regras de decisao
- Markup base operacional entre 30% e 40%, com ajuste por contexto.
- Preco final deve considerar custo do item + frete + markup.
- Pedido com risco tecnico alto pode exigir margem de seguranca maior.
- Item estrategico para relacionamento pode aceitar margem menor mediante aprovacao.

## Composicao do preco final
- Custo direto: preco do fornecedor
- Custo logistico: frete, prazo e complexidade de entrega
- Margem alvo: percentual aplicado sobre custo total
- Ajuste comercial: excecao autorizada por responsavel

## Situacoes que exigem revisao humana
- Margem abaixo do minimo definido para o contexto
- Divergencia relevante entre custo previsto e custo real de entrega
- Pedido com especificacao instavel ou sujeito a retrabalho
- Cliente com condicoes comerciais fora do padrao

## Casos-limite e excecoes
- Urgencia extrema pode elevar custo logistico e reduzir previsibilidade de margem.
- Produto de alta recorrencia pode operar com margem mais calibrada por historico.
- Item de importacao/especialidade deve considerar risco adicional de execucao.

## Sinais praticos para uso do Hermes
- Sempre exibir diferenca entre custo estimado e preco final sugerido.
- Registrar motivo de excecao quando margem fugir do intervalo recomendado.
- Reaproveitar historico de pedidos semelhantes para calibrar markup.

## Paginas relacionadas
- [[infore]]
- [[suprimentos-corporativos]]
- [[cotacao-preco-arbitragem]]
- [[intake-produto-especificacao-estruturada]]
- [[analytics-rentabilidade-fornecedor-margem]]
- [[estoque-just-in-time]]
- [[hermes-agent]]
