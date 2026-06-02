---
title: Intake de Produto e Especificacao Estruturada
created: 2026-06-02
updated: 2026-06-02
type: process
tags: [intake, especificacao, cotacao, qualidade-dados, hermes-agent]
sources: [PLANO_AJUSTES_MVP.md, visita-relatorios/dia-28-05-26/05-28 Abastecimento sob demanda para servicos maritimos_ padronizacao de intake, arbitragem de preco e mitigacao de riscos de especificacao-Summary (1).md]
confidence: high
---

# Intake de Produto e Especificacao Estruturada

## Definicao e objetivo
O intake estruturado e a etapa que transforma uma solicitacao de compra em dados suficientes para uma cotacao confiavel. O objetivo e reduzir ambiguidade, evitar retrabalho e aumentar a taxa de acerto do [[hermes-agent]].

## Contexto operacional Infore
Na rotina da [[infore]], muitos pedidos chegam com descricao incompleta. Isso alonga o ciclo de [[cotacao-preco-arbitragem]], aumenta erros de comparacao e afeta a [[precificacao-markup-margem]].

## Campos essenciais de intake
- Nome do produto
- Quantidade e unidade
- Especificacoes tecnicas minimas (medida, material, potencia, capacidade, etc.)
- Marca/modelo de referencia (quando houver)
- Link de referencia (quando houver)
- Contexto de uso (ex.: escritorio, manutencao, maritimo)
- Restricao de qualidade ou norma (quando aplicavel)
- Imagem do item (quando aplicavel)

## Regras de decisao
- Se nome + quantidade + unidade estiverem ausentes, bloquear envio para cotacao.
- Se especificacao tecnica estiver incompleta e houver risco de compra errada, solicitar complemento antes de pesquisar.
- Se houver link de referencia valido, priorizar essa informacao para compor a busca.
- Se houver marca preferencial do cliente, considerar como criterio de comparacao e nao apenas de preco.

## Checklist de completude antes da cotacao
- O item esta identificavel sem interpretacao subjetiva?
- A unidade esta correta para o tipo de produto?
- Existe especificacao minima para diferenciar variacoes semelhantes?
- Ha indicacao de marca/modelo ou equivalente aceito?
- Existe prazo/criticidade da compra informado?

## Casos-limite e excecoes
- Pedido urgente com dados incompletos: cotar com melhor esforco, mas sinalizar baixa confianca.
- Produto tecnico com norma obrigatoria: nao avancar sem requisito normativo minimo.
- Item sem marca e sem especificacao: classificar como alto risco de erro e exigir validacao humana.

## Sinais praticos para uso do Hermes
- Quanto maior a qualidade do intake, maior a confianca da recomendacao.
- Itens com baixa especificacao devem gerar alerta de ambiguidade.
- Pedidos recorrentes devem reaproveitar padrao de especificacao historico.

## Paginas relacionadas
- [[infore]]
- [[suprimentos-corporativos]]
- [[atendimento-consultivo]]
- [[cotacao-preco-arbitragem]]
- [[precificacao-markup-margem]]
- [[hermes-agent]]
