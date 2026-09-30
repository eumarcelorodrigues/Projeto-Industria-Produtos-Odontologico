# Projeto-Industria-Produtos-Odontologico

📊 Dashboard de Visão do Negócio — Indústria de Produtos Odontológicos

Este repositório contém a solução completa de Business Intelligence para análise comercial e financeira de uma Indústria de Produtos Odontológicos. O projeto abrange desde o pipeline de ETL (Extração, Transformação e Carga) via Linguagem M no Power Query até a modelagem dimensional e construção do dashboard interativo no Power BI.

📌 Visão Geral do Projeto

A solução foi projetada para oferecer visibilidade estratégica sobre o desempenho de orçamentos, contratos aprovados, canais de distribuição (revendas) e cobertura geográfica de vendas no mercado odonto-industrial.

🎯 Principais Indicadores (KPIs)

Receita Orçada: R$ 1,61 Trilhão (Volume total de cotações emitidas).

Receita Aprovada: R$ 408,53 Bilhões (Conversão real em vendas).

Ticket Médio: R$ 1,18 Milhão por operação.

Taxa de Aprovação: 25,3% de conversão dos orçamentos gerados.

Crescimento YoY: +58,6% de variação percentual na receita em comparação ao ano anterior.

🛠️ Arquitetura da Solução e Engenharia de Dados

1. Tratamento de Dados (Power Query & Linguagem M)

Toda a etapa de higienização, estruturação e transformação dos dados foi realizada utilizando rotinas customizadas em Linguagem M:

Limpeza e Padronização: Removidos espaços extras (Text.Trim) e padronizadas as caixas de texto (Text.Proper) para clientes, distribuidores e produtos.

Tratamento de Nulos: Células vazias em colunas críticas foram substituídas por "Não Informado" ou 0 para preservar a integridade das somatórias.

Conversão e Parsing de Datas: Garantida a tipagem estrita de datas para prevenir quebras no pipeline de Inteligência Temporal.

Modelagem Dimensional (Star Schema):

Tabela Fato (fOrcamentos): Contém os registros de cotações, quantidades, valores e status.

Tabelas Dimensão (dCliente, dVendedor, dProduto, dCalendario): Estrutura normalizada com chaves substitutas (Surrogate Keys) para otimização do modelo de dados.

📐 Estrutura do Dashboard (Power BI)

O painel foi estruturado visualmente para cobrir as principais perguntas de negócio:

Visão de Performance Mensal:

Gráfico comparativo de linha/barra mostrando a evolução da Receita Orçada vs. Receita Aprovada ao longo dos meses.

Análise por Cliente / Clínica:

Tabela detalhada indicando os maiores valores aprovados e orçados por conta.

Distribuição Geográfica:

Mapa de bolhas (Microsoft Azure Maps) para identificar a concentração de vendas por estado e região.

Performance por Revenda e Status:

Ranking de faturamento das principais revendas/distribuidoras parceiras (Dental Cremer, Dental Excellence, etc.).

Funil de orçamentos categorizado por status (Aprovado, Reprovado, Cancelado, Em Análise).

💻 Como Reproduzir este Projeto

Pré-requisitos

Microsoft Power BI Desktop (versão mais recente recomendada).

Arquivo de dados-fonte em formato Excel/CSV ou banco de dados relacional.

Passo a Passo

Clone este repositório:

git clone https://github.com/seu-usuario/seu-repositorio.git


Abra o arquivo .pbix na pasta raiz usando o Power BI Desktop.

Caso precise redefinir o caminho do arquivo fonte:

Vá em Transformar Dados > Configurações da Fonte de Dados.

Altere o caminho para a localização do seu arquivo de dados local.

✒️ Autor

Desenvolvido por Marcelo Rodrigues.

Conecte-se comigo no LinkedIn! https://www.linkedin.com/in/marcelordasilva/
