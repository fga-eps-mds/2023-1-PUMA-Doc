# Análise de Valor Agregado

## 1. Introdução

Análise de Valor Agregado (AVA) ou Earned Value Analysis (EVA) é uma técnica introduzida no governo dos Estados Unidos na década de 60 por meio do Departamento de Defesa. Essa técnica utiliza a comparação da progressão de avanço físico do projeto com relação ao planejado para a integração do escopo, prazo e custo. Dessa forma, a Análise de Valor Agregado permite estabelecer uma razão entre o custo real aplicado e o produto físico obtido.

## 2. Detalhamento do AVA - PUMA

O objetivo da Análise de Valor Agregado é integrar as medições de Cronograma, Escopo e Custo para estabelecer uma relação entre o produto obtido e os custos reais.

Dessa forma, no desenvolvimento do diagrama, foram utilizadas as seguintes informações sobre o projeto:

- Quantidade de Sprints ou Iterações do projeto ou release;
- Quantidade de Sprints ou Iterações concluídas até o momento;
- Esforço total necessário para concluir o projeto ou release;
- Esforço concluído até o momento;
- Orçamento do projeto ou da release;
- Valor gasto até o momento.

## 3. Parâmetros Gerais do Projeto

- IDC - Índice de Desempenho de Custos;
- IDP - Índice de Desempenho de Prazo;
- VDC - Variação de Desempenho de Custo;
- VDP - Variação de Desempenho de Prazo.

## 4. Parâmetros das Releases

- PPR - Pontos Planejados por Release;
- PCR - Pontos Concluídos por Release;
- OER - Orçamento Estimado por Release;
- CA - Custo até o momento;
- VPR - Valor Planejado por Release;
- VAR - Valor Agregado por Release.

## 5. Parâmetros das Sprints

- PPS - Pontos Planejados por Sprint;
- PCS - Pontos Concluídos por Sprint;
- PIS - Pontos Incompletos por Sprint;
- PAS - Pontos Adicionados por Sprint;
- OGS - Orçamento Gasto por Sprint;
- TSC - Total de Sprints Concluídas;
- TSE - Total de Sprints Estimadas;

## 3. Parâmetros EVM
- OER = Orçamento estimado para a Release;
- CA = VAR / OER (Custo até o momento);
- VPR = OER * (TSC / TSE) (Valor Planejado);
- VAR = OER * (PCR / PPR) (Valor Agregado);
- IDC = VAR / CA (Índice de Desempenho de Custos);
- VDC = VAR - CA (Variação de Desempenho de Custos);
- IDP = VAR / VPR (Índice de Desempenho de Prazo);
- VDP = VAR - VPR (Variação de Desempenho de Prazo).

Abaixo, temos o projeto EVM:

<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vTeyyjcRczmB8lPCnsIzKBswJdSccMxqCAoPJhWVL0P4Yfg90ePOyIYYifIfI-s_PgwYT7qr8HkKTyl/pubhtml?widget=true&amp;headers=false"></iframe>

## Histórico de Revisão

| Data       | Versão |      Modificação      |    Autor     |
| :--------- | :----- | :-------------------- | :----------- |
| 28/05/2023 | 0.1    | Abertura do documento | Guilherme Daniel Fernandes da Silva |
| 08/06/2023 | 0.5    | Adição do projeto EVM | Ítalo Alves Guimarães e Guilherme Daniel Fernandes da Silva |
