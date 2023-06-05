# Plano de Gerenciamento de Qualidade

## Introdução

A ISO/IEC 25000 (SQuaRE) fornece diversas diretrizes para a avaliação da qualidade de software em diferentes aspectos. Ela estabelece um conjunto de características de qualidade, como funcionalidade, confiabilidade, usabilidade, eficiência, manutenibilidade e portabilidade.

Já a ISO/IEC 25010, disponibilizada, estabelece um modelo para a qualidade do produto de software, definindo como características de qualidade: adequação funcional, desempenho, compatibilidade, usabilidade, segurança, manutenibilidade e portabilidade. 

## Objetivo 

Esse documento tem como objetivo especificar as ferramentas que serão utilizadas, bem como as métricas que serão analisadas com o objetivo de definir os critérios de qualidade do projeto.

## Qualidade

### Qualidade Interna
Refere-se às características do software que não são visíveis para os usuários finais. Dessa forma, está relacionada à estrutura interna do software, sua manutenibilidade, facilidade de modificação, extensibilidade e outras propriedades técnicas. 

A qualidade interna está focada nos desenvolvedores e equipes de manutenção de software. Assim, temos como exemplos de métricas de qualidade interna: complexidade do código, acoplamento e coesão dos módulos, presença de padrões de projeto, ausência de código duplicado, entre outros. Com isso, uma boa qualidade interna pode facilitar a manutenção do software, melhorar a produtividade da equipe de desenvolvimento e reduzir os custos de correção de defeitos.

### Qualidade Externa
Refere-se às características do software que são diretamente percebidas pelos usuários finais. Desta forma, está relacionada à usabilidade, desempenho, confiabilidade, eficiência e outras propriedades que afetam diretamente a experiência do usuário.

A qualidade externa é voltada para as expectativas e requisitos dos usuários finais do software. Temos como exemplos de métricas de qualidade externa: tempo de resposta, taxa de erros, facilidade de uso, eficiência de recursos, entre outros. Uma boa qualidade externa contribui para a satisfação do usuário, confiabilidade do software e efetividade na realização das tarefas desejadas.

### Qualidade de Uso
Concentra-se em quatro características principais: eficácia, produtividade, segurança e satisfação do usuário, características derivadas da combinação das características de qualidade definidas na ISO.

## Ferramentas

### Testes Unitários (Jest)
Os testes unitários são testes automatizados que visam verificar o funcionamento de pequenas unidades de código, isoladas do restante do sistema (VALENTE, 2020). Para a realização desses testes, a equipe utiliza o Jest, uma ferramenta de código aberto que permite a aplicação de testes em aplicações JavaScript de maneira fácil e simplificada.

### ESLint
O ESLint é uma ferramenta amplamente utilizada para verificação e análise estática de código JavaScript. Ele auxilia os desenvolvedores a garantir a qualidade do código, identificando e reportando possíveis problemas, erros ou más práticas de programação. O ESLint oferece uma variedade de regras configuráveis, que podem ser personalizadas de acordo com as necessidades do projeto, permitindo a aplicação de padrões de codificação consistentes e aprimorando a legibilidade, manutenibilidade e interoperabilidade do código.

### SonarCloud
O SonarCloud é uma ferramenta usada para coletar métricas e indicadores técnicos, permitindo o monitoramento da qualidade do código. Esses dados coletados são usados para auxiliar no planejamento de melhorias na qualidade do código. Durante o desenvolvimento do projeto, foram coletadas métricas após cada Pull Request submetido. Essas métricas foram combinadas para calcular os aspectos de qualidade relevantes para este projeto, que se dividem em confiabilidade e manutenibilidade do código.

## Planejamento

### Modelos e métricas de qualidade
Como modelo de qualidade de software, optamos pela utilização da NBR - ISO/IEC 25010.

| Característica | Subcaracterísticas |
| -------------- | ------------------ |
| Adequação Funcional | Integridade funcional, Correção funcional, Adequação funcional |
| Eficiência de performance | Comportamento do tempo, Uso de recursos, Capacidade |
| Compatibilidade | Coexistência, Interoperabilidade |
| Usabilidade | Adequação reconhecível, Capacidade de aprendizado, Operabilidade, Proteção de erro do usuário, Estética da interface de usuário, Acessibilidade |
| Confiabilidade | Maturidade, Disponibilidade, Tolerância a falhas, Recuperabilidade |
| Segurança | Confidencialidade, Integridade, Ausência de repúdio, Rastreabilidade de uso, Autenticidade |
| Manutenibilidade | Modularidade, Reusabilidade, Analisabilidade, Modificabilidade, Testabilidade |
| Portabilidade | Adaptabilidade, Facilidade de instalação, Capacidade de substituição |

### Métricas de qualidade
As métricas de qualidade definidas para o software são:

| Métrica | Descrição |
| ------- | --------- |
| Bugs    | Quantidade de bugs encontrados |
| Vulnerabilidades | Quantidade de vulnerabilidades encontradas |
| Code Smell | Quantidade de code smell encontrada |
| Coverage | Cobertura de código dos testes |
| Duplicação | Quantidade de linhas de código duplicadas |
| Linhas | Quantidade de linhas de código |
| Security Rating | Avaliação de segurança e falhas | 

Dessa forma, por meio da utilização de métricas, é possível identificar as subcaracterísticas associadas e, assim, avaliar a qualidade do produto. Essa avaliação não apenas proporciona insights sobre a produtividade do projeto, mas também oferece resultados que podem influenciar as decisões tomadas em relação ao seu desenvolvimento.

Foram estabelecidos então valores mínimos aceitáveis para cada métrica do projeto PUMA a partir das métricas especificadas no SonarCloud:

| Métrica | Descrição |
| ------- | --------- |
| Coverage | no mínimo 80% |
| Vulnerabilities | Nota A |
| Bugs | Nota A |
| Security Hotspots | Nota A |
| Code Smells | Nota A |
| Duplication | até 3.0% |

## Controle de qualidade
Para garantir a implementação de procedimentos de qualidade, adotamos as seguintes atividades: documentação, controle de versão, controle de código, controle de commits e testes automatizados. 

Essas tarefas são executadas por meio de ferramentas e sistemas que desempenham um papel fundamental na garantia da qualidade do software.

## Referências

- ISO/IEC 25010. Disponível aqui. Acesso em: 03/06/2023.

- Jest. Disponível aqui. Acesso em: 03/06/2023.

- VALENTE, Marco. Engenharia de Software Moderna: Princípios e Práticas para Desenvolvimento de Software com Produtividade. 2020. Disponível aqui. Acesso em: 03/06/2023.

## Histórico de Revisão

| Data       | Versão |      Modificação      |    Autor     |
| :--------- | :----- | :-------------------- | :----------- |
| 04/06/2023 | 0.1    | Abertura do documento.| Guilherme Daniel Fernandes da Silva |





