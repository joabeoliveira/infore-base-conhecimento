---
title: Integracao Bitrix24, APIs e Workflows
created: 2026-06-02
updated: 2026-06-02
type: process
tags: [bitrix24, integracao, api, workflow, crm]
sources: [bitrix24/MCP/resumo.md, bitrix24/API/pemissoes.md]
confidence: high
---

# Integracao Bitrix24, APIs e Workflows

## Definicao e objetivo
Este no descreve o papel do Bitrix24 no ecossistema Infore 4.0 como camada de CRM e automacao comercial. O objetivo e padronizar como os fluxos de cotacao e acompanhamento se conectam ao sistema.

## Contexto operacional Infore
No processo da [[infore]], o Bitrix24 atua como ponto de registro e acompanhamento comercial antes do fechamento operacional. Ele conecta atendimento, status de negociacao e historico de interacoes.

## Regras de decisao
- Registrar contexto minimo da cotacao antes de avancar para execucao.
- Garantir que campos obrigatorios do funil estejam consistentes com o fluxo real.
- Em caso de conflito entre status comercial e status operacional, priorizar reconciliacao antes de fechar pedido.
- Evitar automacoes que alterem dados criticos sem trilha de auditoria.

## Boas praticas de integracao
- Usar metodos oficiais e documentacao atualizada para evitar chamadas inexistentes.
- Padronizar mapeamento de campos entre CRM e fluxo de cotacao.
- Tratar falhas de API com reprocessamento controlado e log estruturado.
- Separar claramente eventos de leitura (consulta) e escrita (atualizacao).

## Casos-limite e excecoes
- Campo obrigatorio ausente no CRM: bloquear avanco automatico e solicitar complemento.
- Mudanca manual no CRM durante automacao: revalidar estado antes de escrever.
- Falha transiente de API: tentar novamente com politica de retentativa limitada.

## Sinais praticos para uso do Hermes
- O Hermes deve explicitar quando uma recomendacao depende de dado comercial ausente no CRM.
- O Hermes deve sinalizar divergencia entre informacao do CRM e do fluxo de cotacao.
- O Hermes deve orientar revisao humana em atualizacoes com alto impacto comercial.

## Paginas relacionadas
- [[infore]]
- [[fluxo-pedidos-vendedor-comprador]]
- [[cotacao-preco-arbitragem]]
- [[automacao-n8n-workflows-integracao]]
- [[integracao-cplus5-erp-legado]]
- [[hermes-agent]]
