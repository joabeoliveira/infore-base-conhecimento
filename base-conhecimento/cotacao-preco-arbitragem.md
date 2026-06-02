---
title: Cotacao de Preco e Arbitragem
created: 2026-06-02
updated: 2026-06-02
type: process
tags: [cotacao, arbitragem, fornecedores, pesquisa, decisao-comercial]
sources: [PLANO_AJUSTES_MVP.md, visita-relatorios/dia-28-05-26/05-28 Analise do Fluxo de Pedidos_ Ineficiencias e Dependencia Manual no Processo de Vendas-Summary.md, visita-relatorios/dia-28-05-26/lista-maior-para-o-menor-fornecedores-por-quantidade-compras.csv]
confidence: high
---

# Cotacao de Preco e Arbitragem

## Definicao e objetivo
A arbitragem de preco e a pratica de comparar multiplas fontes para encontrar a melhor combinacao entre custo, prazo e confiabilidade. O objetivo na [[infore]] nao e apenas menor preco, mas melhor decisao comercial.

## Contexto operacional Infore
No fluxo atual de [[suprimentos-corporativos]], a pesquisa manual consome tempo e depende da experiencia individual. Com o [[hermes-agent]], a cotacao deve ser acelerada e mais consistente, desde que o [[intake-produto-especificacao-estruturada]] esteja bem preenchido.

## Regras de decisao
- Comparar no minimo 3 fontes quando houver oferta suficiente.
- Priorizar fontes que a infore já tenha comprado historicamente, quando aplicavel e, as que a infore possui link de afiliado, quando aplicavel. 
- Priorizar fontes com historico positivo e boa aderencia ao item solicitado.
- Nao escolher oferta apenas por preco se houver risco de especificacao incorreta.
- Sempre considerar disponibilidade e prazo junto com valor.

## Heuristicas de selecao de fornecedor
- Fornecedor recorrente com bom historico pode ganhar prioridade em empate tecnico.
- Marketplace com melhor cobertura pode ser ponto de partida, mas nao criterio unico.
- Fornecedor especialista por categoria pode superar oferta mais barata de fonte generica.

## Criterios de fallback
- Se nao houver 3 fontes validas, registrar justificativa de baixa amostragem.
- Se houver alta dispersao de preco, pedir revisao humana antes de fechar.
- Se dados de entrada estiverem incompletos, retornar solicitacao de complemento ao [[atendimento-consultivo]].

## Casos-limite e excecoes
- Item de alta urgencia: usar melhor fonte disponivel com anotacao de risco.
- Item com exigencia tecnica/normativa: restringir comparacao apenas a fornecedores aderentes.
- Item raro sem referencia confiavel: elevar para analise especializada.

## Sinais praticos para uso do Hermes
- A confianca da recomendacao cai quando faltam fontes ou especificacoes.
- Divergencia extrema entre ofertas sugere erro de matching ou produto diferente.
- Historico de compras recorrentes, que podem ser consultadas no banco de dados, ajuda a reduzir variancia de decisao.

## Paginas relacionadas
- [[infore]]
- [[fornecedores-ranking-relacionamento]]
- [[fluxo-pedidos-vendedor-comprador]]
- [[intake-produto-especificacao-estruturada]]
- [[precificacao-markup-margem]]
- [[logistica-regional]]
- [[hermes-agent]]
