# Base de conhecimento do projeto Infore 4.0
## Resumo
Esta base de conhecimento reúne os principais conceitos, processos e informações relacionados ao projeto Infore 4.0, que tem como objetivo desenvolver um motor de IA para automação de cotações na empresa Infore. A base de conhecimento é organizada em diferentes categorias, como entidades, conceitos e processos, e inclui informações sobre a empresa Infore, seus serviços, seus fluxos de trabalho e outras informações relevantes para criar uma memória persistente para o Hermes Agent, que é o assistente virtual utilizado para auxiliar a equipe de compras e demais setores envolvidos.

A ideia é manter uma base de conhecimento atualizada e estruturada, que possa ser facilmente acessada e utilizada pelo Hermes Agent para fornecer insights, análises e recomendações durante o desenvolvimento do projeto INFORE 4.0. A base de conhecimento é um recurso valioso para garantir que o desenvolvimento do projeto seja eficiente, alinhado com as necessidades da Infore e baseado em dados e informações relevantes.

## Fontes iniciais
- Documentação da API do Bitrix24
- Roteiro de visita presencial à Infore
- Relatórios de visitas anteriores
- Entrevistas com colaboradores da Infore

## Páginas Relacionadas existentes
- [[infore]]
- [[suprimentos-corporativos]]
- [[logistica-regional]]
- [[atendimento-consultivo]]
- [[estoque-just-in-time]]
- [[hermes-agent]]

## Novos nós (Trilha Comercial)
Esta trilha organiza o núcleo operacional da automação de cotações: qualidade do intake, comparação de ofertas e formação de preço final.

- [[intake-produto-especificacao-estruturada]] - Padroniza a entrada dos pedidos para reduzir ambiguidade e retrabalho.
- [[cotacao-preco-arbitragem]] - Define critérios para comparação de fontes e seleção da melhor proposta.
- [[precificacao-markup-margem]] - Consolida regras de markup e margem para proteger rentabilidade.

## Novos nós (Trilha Operacional)
Esta trilha consolida o fluxo ponta a ponta entre vendedor e comprador e os critérios de priorização de fornecedores.

- [[fluxo-pedidos-vendedor-comprador]] - Organiza as etapas do pedido e os pontos de validação para reduzir ruído operacional.
- [[fornecedores-ranking-relacionamento]] - Estrutura ranking e critérios de escolha com base em histórico, confiabilidade e margem.

## Novos nós (Trilha Especialidades)
Esta trilha cobre cenários de maior risco operacional, com regras adicionais de decisão e conformidade.

- [[operacao-paraguai-especialista]] - Documenta o fluxo de compras no Paraguai e o risco de dependência de especialista.
- [[abastecimento-demanda-sourcing-heterogeneo]] - Organiza sourcing por categoria em demandas heterogêneas e de alta variabilidade.
- [[conformidade-normas-por-categoria]] - Define critérios mínimos de conformidade para reduzir erro e devolução.

## Novos nós (Trilha Integracoes)
Esta trilha organiza a orquestracao entre CRM, automacao e ERP para sustentar o fluxo operacional ponta a ponta.

- [[integracao-bitrix24-apis-workflows]] - Define como o CRM entra no processo comercial e de acompanhamento de cotacoes.
- [[integracao-cplus5-erp-legado]] - Consolida regras para persistencia transacional de orcamentos e vendas no ERP.
- [[automacao-n8n-workflows-integracao]] - Estrutura workflows de automacao e tratamento de falhas entre sistemas.

## Novos nós (Trilha Analytics)
Esta trilha fecha o ciclo de melhoria continua, conectando decisao de fornecedor com resultado de margem e rentabilidade.

- [[analytics-rentabilidade-fornecedor-margem]] - Organiza indicadores e regras de leitura para equilibrar volume, margem e risco por fornecedor.


