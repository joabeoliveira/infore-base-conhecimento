---
title: Integracao CPLUS 5 e ERP Legado
created: 2026-06-02
updated: 2026-06-02
type: process
tags: [cplus5, erp, integracao, orcamentos, vendas]
sources: [CPLUs/Infore 4.0 - Questionario Tecnico CPLUS 5 (25-05-2026).md]
confidence: high
---

# Integracao CPLUS 5 e ERP Legado

## Definicao e objetivo
Este no descreve a integracao do CPLUS 5 como sistema de gestao central para cadastro, orcamentos e vendas. O objetivo e garantir consistencia entre automacao de cotacao e registro transacional no ERP.

## Contexto operacional Infore
No fluxo da [[infore]], o CPLUS tende a entrar nas etapas de consolidacao e formalizacao. A qualidade dos dados vindos de [[fluxo-pedidos-vendedor-comprador]] e essencial para evitar retrabalho no ERP.

## Regras de decisao
- Tratar CPLUS como fonte transacional final para registros formais.
- Validar IDs, campos obrigatorios e formato antes de enviar dados.
- Priorizar endpoints de orcamentos e vendas no MVP de cotacao.
- Em caso de inconsistencias, interromper escrita e encaminhar para revisao.

## Escopo funcional relevante
- Produtos: consulta e manutencao de catalogo quando necessario.
- Orcamentos: criacao e consulta para suportar processo comercial.
- Vendas: conversao e acompanhamento de fechamento.
- Clientes e fornecedores: manutencao cadastral e vinculos.

## Casos-limite e excecoes
- Endpoint indisponivel: manter fila de reenvio com controle de duplicidade.
- Mudanca de schema/campo: versionar mapeamentos e validar compatibilidade.
- Dado parcial vindo de origem: nao persistir sem campos minimos do ERP.

## Sinais praticos para uso do Hermes
- O Hermes deve indicar quando a recomendacao ainda nao esta pronta para persistencia no ERP.
- O Hermes deve explicitar quais dados faltam para criar orcamento/venda sem erro.
- O Hermes deve sinalizar risco quando houver divergencia entre cotacao e cadastro mestre.

## Paginas relacionadas
- [[infore]]
- [[fluxo-pedidos-vendedor-comprador]]
- [[precificacao-markup-margem]]
- [[integracao-bitrix24-apis-workflows]]
- [[automacao-n8n-workflows-integracao]]
- [[hermes-agent]]
