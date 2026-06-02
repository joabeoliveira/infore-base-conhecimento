---
title: Automacao n8n e Workflows de Integracao
created: 2026-06-02
updated: 2026-06-02
type: process
tags: [n8n, automacao, workflow, orquestracao, integracao]
sources: [infraestrutura/n8n/resumo.md, n8n/README.md]
confidence: medium
---

# Automacao n8n e Workflows de Integracao

## Definicao e objetivo
Este no define o papel do n8n como camada de orquestracao entre sistemas no Infore 4.0. O objetivo e automatizar passagens de contexto entre CRM, motor de cotacao e ERP com rastreabilidade.

## Contexto operacional Infore
A operacao da [[infore]] envolve varios sistemas e canais. O n8n ajuda a reduzir tarefas repetitivas, acionar integracoes e padronizar etapas de execucao do [[fluxo-pedidos-vendedor-comprador]].

## Regras de decisao
- Cada workflow deve ter gatilho, validacao e saida claramente definidos.
- Nao propagar evento para proxima etapa sem validacao minima dos dados.
- Toda escrita em sistema externo deve gerar log de sucesso ou erro.
- Falhas devem ser tratadas com retentativa controlada e fila de reprocesso.

## Padroes de workflow
- Entrada: captura de evento comercial ou operacional.
- Transformacao: normalizacao de payload e enriquecimento de contexto.
- Integracao: chamada a APIs externas conforme regra do processo.
- Saida: atualizacao de status e notificacao de resultado.

## Casos-limite e excecoes
- Evento duplicado: aplicar idempotencia para evitar processamento duplo.
- Dependencia externa indisponivel: reencaminhar para fila e notificar.
- Payload incompleto: interromper fluxo e pedir complemento de origem.

## Sinais praticos para uso do Hermes
- O Hermes deve informar em qual etapa do workflow ocorreu falha.
- O Hermes deve separar erro de dados de erro de integracao.
- O Hermes deve recomendar acao de reprocesso quando apropriado.

## Paginas relacionadas
- [[infore]]
- [[fluxo-pedidos-vendedor-comprador]]
- [[integracao-bitrix24-apis-workflows]]
- [[integracao-cplus5-erp-legado]]
- [[cotacao-preco-arbitragem]]
- [[hermes-agent]]
