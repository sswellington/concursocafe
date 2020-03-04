# Banco de Dados

# Modelagem Conceitual - ER

## Redundância de Dados

* Redundância controlada de dados:

Acontece quando o software tem conhecimento da múltipla representação da informação e garante a sincronização entre as diversas representações.

* Redundância não controlada de dados:

Acontece quando a responsabilidade pela manutenção da sincronia entre as diversas representações de uma informação está com o usuário e não com o software.

A solução para evitar a redundância não controlada de informações é o Compartilhamento de dados. Nesta forma de processamento, cada informação é armazenada uma única vez, sendo acessado pelos vários sistemas que dela necessitam.

[Fonte:](https://docente.ifrn.edu.br/josecunha/disciplinas/banco-de-dados/material-de-aula/introducao-bd)

## Modelos de Dados

**Objetivo** de *representar* o banco de dados. 

> Os modelos, gradativamente, aprofundam seus níveis de detalhes. Podemos utilizar um projeto de banco de dados para explicar: primeiro nós fazemos um levantamento de inicial que tende a ser de alto nível e ter maior abstração (modelagem conceitual - modelo entidade relacionamento), depois nós nos aprofundamos nos detalhes e definimos um paradigma (modelagem lógica ou representativa ou de implementação - modelo relacional) e, por fim, nós chegamos no nível mais baixo de abstração, mostramos detalhes de um SGBD específico (Oracle, por exemplo).

* **CONCEITUAL / de alto nível:** 
Modo como usuários percebem os dados.

* **REPRESENTATIVO / de implementação / modelo lógico:** 
oferece conceitos que podem ser entendidos pelos usuários, 
mas não está muito longe de como os dados são organizados e armazenados no computador.

* **FÍSICO / de baixo nível:**
detalhes de como os dados são armazenados.

## Arqutitetura de Três Esquemas

**Objetivo** obter a *independência* entre as camadas. Ou seja, o nível interno poderá ser alterado sem afetar o nível conceitual, bem como o nível conceitual pode ser alterado sem alterar o nível externo.


* **Nível externo ou de visão:** 
inclui uma série de esquemas externos ou visões do usuário. Cada esquema externo descreve a parte do banco de dados em que um grupo de usuários em particular está interessado e oculta o restante do banco. 
(*) Um modelo representativo é usado para descrever o esquema externo.

* **Nível conceitual:** 
tem esquema conceitual, que descreve a estrutura do banco de dados inteiro para uma comunidade de usuários. Oculta detalhes das estruturas de armazenamento físico e se concentra na descrição das entidades, tipos de dados, relacionamentos, operações e restrições.
(*) Um modelo representativo é usado para descrever o esquema conceitual.

* **Nível interno:** 
tem um esquema interno, que descreve a estrutura do armazenamento físico do banco de dados. 
(*) Usa um modelo de dados físico e descreve detalhes completos do armazenamento de dados.