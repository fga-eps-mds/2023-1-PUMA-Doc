# Plano de Contribuição

## Introdução

Este Plano de Contribuição determina as regras para submissão de códigos e contribuições nos repositórios do Projeto PUMA no semestre 2023-1.

## Issues

Todas as contribuições devem estar vinculadas a uma única _issues_, e todas as _issues_ devem ser criadas e preenchidas de acordo com os templates disponíveis no repositório.

Cada _issue_ também deve possuir _Assignees_, responsáveis por desenvolvê-la, e _labels_ para indicar o tipo de _issue_.

## Commits

Os _commits_ devem ser na língua inglesa, curtos e simples, de forma a expor objetivamente o trabalho que foi feito naquele _commit_.

Caso o _commit_ seja resultado de um trabalho em equipe, deve-se utilizar o _Co-authored-by:_

Visando uma melhor padronização, utilizaremos o commit semântico, que pode ser conferido e acessado através deste [link](https://www.letscode.com.br/blog/o-que-sao-commits-semanticos-e-como-utilizo).

Como utilizar

Os commits semânticos possuem um esqueleto padrão que consiste em partes opcionais que podem ou não ser acrescentadas.

```
<tipo>: <descrição>

Exemplo:
Fix: Corrigindo redirecionamento de usuario ao se cadastrar na plataforma
```

A primeira e principal descrição de um commit semântico é o Tipo. Tem como finalidade dizer o que aquele commit está realizando. Os tipos se resumem em feat, fix, refactor, style, chore, doc e test [[1]](#ref1).

```
Feat: Utilizado quando feita qualquer adição ao código.O foco dele é ser usado quando houver uma nova implementação de funcionalidade no sistema.
Fix: Utilizado quando existem erros no código que estão causando bugs.
Refactor: Utilizado na refatoração de código mas que não altere sua funcionalidade.
Style: Utilizado quando feita uma alteração no estilo e formatação do código.
Chore: Utilizado na atualização para mudanças em ferramentas, configurações e bibliotecas. Atualizações que não ocasionam em alteração no código de produção.
Doc: Utilizado quando é adicionado ou atualizado alguma documentação no projeto.
Test: Utilizado quando feita qualquer alteração em relação aos testes do projeto.
```

## Pull Requests

Os _pull requests_ devem estar obrigatoriamente vinculados a uma _issue_. É necessário também a inclusão de _Reviewers_, responsáveis por verificar a conclusão da _issue_ e a validade do _pull request_. O _pull request_ só poderá ser mergeado com a aprovação de pelo menos dois _Reviewers_.

## Branches

Com exceção das _branches_ principais (_main, gh-pages, devel_), cada _branch_ deve estar vinculada a uma única _issue_. Após a conclusão da _issue_ e fechamento do _pull request_ associado, a _branch_ referente não pode ser apagada, porque ela será utilizada para organização de pacotes de entregas para a release. Para uma correta padronização das branchs e fluxo, utilizaremos o [Gitflow](https://www.atlassian.com/br/git/tutorials/comparing-workflows/gitflow-workflow#:~:text=O%20que%20%C3%A9%20o%20Gitflow,por%20Vincent%20Driessen%20no%20nvie.) [[2]](#ref2).

![Gitflow](../assets/gitflow.svg)

Para manter o padrão criaremos a branch bem parecido com o commit, sendo adotado os seguintes padrões:

```
<tipo>/<descrição>

Exemplo:
feature/migracao-orm
fix/redirecionamento-usuario
hotfix/redirecionamento-senha


feature: Utilizado quando feita qualquer nova implementação de funcionalidade no sistema.
fix: Utilizado quando é necessário abrir uma branch de correção de uma funcionalidade já existente no sistema.
refactor: Utilizado quando é necessário abrir uma branch de refatoração de código mas que não altere sua funcionalidade.
documentation: Utilizado quando é necessário abrir uma branch de documentação no projeto.
hotfix: Utilizado quando é necessário abrir uma branch de correção de um bug em produção no projeto.
```

## Referência

<a id="ref1"></a>
[1] O que são Commits Semânticos e como utilizo?. Disponível em: <https://www.letscode.com.br/blog/o-que-sao-commits-semanticos-e-como-utilizo>. Acesso em: maio, 2023.

<a id="ref2"></a>
[2] Fluxo de trabalho de Gitflow. Disponível em: <https://www.atlassian.com/br/git/tutorials/comparing-workflows/gitflow-workflow#:~:text=O%20que%20%C3%A9%20o%20Gitflow,por%20Vincent%20Driessen%20no%20nvie.>. Acesso em: maio, 2023.

## Histórico de Revisão

| Data       | Versão | Modificação                     | Autor        |
| :--------- | :----- | :------------------------------ | :----------- |
| 05/05/2023 | 0.1    | Abertura do documento.          | Abner Filipe |
| 05/05/2023 | 0.2    | Correção e revisão do documento | Rafael Leão  |
