<h1 align="center">Fundamentos Arquitetura de Software</h1>

<p align="center">Projeto sobre os Fundamentos de Arquitetura de Software onde documento os conceitos fundamentais de OOP - SOLID - Dependency Injection - Clean Code - Design Patterns</p>

---

### :dart: Objetivo

Tenho como objetivo implementar uma documentação a respeito dos fundamentos de software para que possa servir de estudo e consulta sobre o tema abordado. Trata-se de uma aplicação que tem **somente** como propósito a **descrição e exemplificação** dos temas abordados. Desenvolvida em C# com os conceitos fundamentais de OOP - SOLID - Dependency Injection - Clean Code - Design Patterns

### Clone

Clone este repositório em sua máquina local usando:  

```
git clone https://github.com/YuriSiman/software-architecture-fundamentals.git
```

### :pencil2: Tópicos

- [x] [OOP](https://github.com/YuriSiman/software-architecture-fundamentals#oop)  
- [x] [SOLID](https://github.com/YuriSiman/software-architecture-fundamentals#solid)  
- [x] [Clean Code](https://github.com/YuriSiman/software-architecture-fundamentals#clean-code)  
- [x] [Design Patterns](https://github.com/YuriSiman/software-architecture-fundamentals#design-patterns)  

---

## :rocket: Vamos Começar 

## O que é Arquitetura?

"Arquitetura é a organização fundamental de um sistema incorporada em seus componentes, relacionamentos com o ambiente e os princípios que conduzem seu design e evolução."   [ISO/IEC/IEEE 42010-2011](https://www.iso.org/standard/50508.html)

Como construir software:

<img src="./readme-images/arquitetura-software.png" />

### TOGAF

The Open Group Architecture Framework (TOGAF) é um framework de arquitetura corporativa que provê uma abordagem global ao design, planejamento, implementação e governança de uma arquitetura corporativa.

[OpenGroup](https://www.opengroup.org/togaf)

### ISO/IEC/IEEE 42010-2011

Engenharia de sistemas e software ISO / IEC / IEEE 42010 - A descrição da arquitetura é um padrão internacional para descrições de arquitetura de sistemas e software.

[ISO/IEC/IEEE 42010-2011](https://www.iso.org/standard/50508.html)  

[Voltar ao Início](https://github.com/YuriSiman/software-architecture-fundamentals#fundamentos-arquitetura-de-software)  

---

## OOP

É essencial possuir um claro conhecimento dos princípios da orientação a objetos para poder aplicar as melhores práticas de design de código, padrões e abordagens de arquitetura. Na orientação a objetos devemos sempre buscar o baixo acoplamento e a alta coesão entre os objetos, ou seja, evitar uma dependência direta entre um objeto e outro, tendo os objetos executando uma única responsabilidade livres de uma dependência direta com outros.

Pilares da Programação Orientada a Objetos


<img src="./readme-images/pilares-oop.png" />

[Visualizar Código](https://github.com/YuriSiman/software-architecture-fundamentals/tree/master/OOP)  
[Voltar ao Início](https://github.com/YuriSiman/software-architecture-fundamentals#fundamentos-arquitetura-de-software)  

---

## SOLID

<img src="./readme-images/solid.png" />

SOLID é um acrônimo dos cinco primeiros princípios da programação orientada a objetos e design de código identificados por Robert C. Martin (Uncle Bob) por volta do ano 2000. Os princípios SOLID devem ser aplicados para se obter os benefícios da orientação a objetos, como:

- Seja fácil de se manter, adaptar e se ajustar às alterações de escopo
- Seja testável e de fácil entendimento
- Seja extensível para alterações com o menor esforço necessário
- Que forneça o máximo de reaproveitamento
- Que permaneça o máximo de tempo possível em utilização

Problemas comuns que conseguimos evitar quando utilizamos os princípios SOLID:

- Dificuldade na testabilidade / criação de testes de unidade
- Código macarrônico, sem estrutura ou padrão
- Dificuldades de isolar funcionalidades
- Duplicação de código, uma alteração precisa ser feita em N pontos
- Fragilidade, o código quebra facilmente em vários pontos após alguma mudança 

### SRP - Single Responsability Principal

Uma classe deve ter **um,e apenas um,** motivo para ser modificada.

### OCP - Open Closed Principle

Entidades de software (classes, módulos, funções, etc...) devem estar abertas para extensão, mas fechadas para modificação.

### LSP - Liskov Substitution Principle

O principal objetivo do LSP é questionar se o desenvolvedor está realizando uma herança dentro dos padrões de design e abstração ou está apenas seguindo a linha do "é um...". Subclasses devem ser substituíveis por suas Superclasses. Este princípio reswolve o problema de heranças que não deveriam ser implementadas.

Se q(x) é uma propriedade demonstrável dos objetos x de tipo T. Então q(y) deve ser verdadeiro para objetos y de tipo S onde S é um subtipo de T.

### ISP - Interface Segregation Principle

Clientes não devem ser forçados a depender de métodos que não usam. Muitas interfaces específicas são melhores do que uma interface única. Delegar contratos (interfaces) é uma forma de garantir  design e abstração do código.

### DIP - Dependency Inversion Principle

Módulos de alto nível não devem depender de módulos de baixo nível. Ambos devem depender de abstrações. Abstrações não devem depender de detalhes. Detalhes devem depender de abstrações.

Dependa de uma abstração e não de uma implementação.

[Visualizar Código](https://github.com/YuriSiman/software-architecture-fundamentals/tree/master/SOLID)  
[Voltar ao Início](https://github.com/YuriSiman/software-architecture-fundamentals#fundamentos-arquitetura-de-software)  

---

## Clean Code

### O que é um código limpo?

- Simples
- Direto
- Eficiente
- Sem duplicidade
- Elegante
- Feito com cuidado
- Fácil de ler

"Qualquer tolo consegue escrever código que um computador entenda. Bons programadores escrevem código que humanos possam entender".  
Martin Fowler

### Quanto custa um código ruim?

- Alta rotatividade
- Demora na entrega de novas funcionalidades
- Dificuldade na manutenção
- Alta incidência de bugs
- Perda de confiança do cliente
- Desmotivação profissional
- Mais tempo depurando o código do que escrevendo

### Como medir um bom código?

- Quantidade de linhas de código (Devemos buscar reduzir ao máximo o tamanho do código, dependendo do projeto)
- Número de métodos (Devemos buscar utilizar a maior quantidade de métodos para um desacoplamento maior)
- Número de classes (Devemos buscar utilizar a maior quantidade de métodos para um desacoplamento maior)
- Linhas de código por método (Devemos buscar reduzir a quantidade de linhas dentro do método)
- Complexidade ciclomática (Evitar uma grande quantidade de caminhos de execução independentes, ou seja, evitar if's encadeados)
- Número de estruturas de decisão (Evitar um exagero de estruturas de decisão)
- Escolher os nomes que revelem intenção (Revelando o motivo dele existir, o que faz e como é usado. Utilizar nomes fáceis de se encontrar, evitando siglas ou acrônimos. Não economizar palavras para dar nome a alguma coisa)

### Boas práticas

- Nome de classes devem ser substantivos e não devem conter verbos. Ex: ClienteRepository
- Nomes de métodos devem conter verbos de preferência no infinitivo. Ex: AdicionarCliente
- Não ser genérico. Ex: ProcessarFolhaPagamento / CalcularImpostoRenda
- Menos é mais! "A primeira regra dos métodos é que eles devem ser pequenos. A segunda regra é que eles devem ser menores ainda". Uncle Bob
    - Métodos <= 20 linhas
    - Linha <= 100 caracteres
    - Classe <= 500 linhas
- Extraia trechos de métodos privados
- Métodos devem fazer apenas uma coisa, fazê-la certa e somente fazê-la
- Evite muitos parâmetros em métodos
- Não deixe o método mentir dizendo que faz uma coisa mas na verdade faz outras "escondidas"
- Se o método tiver mais de uma responsabilidade, extraia em dois ou mais
- Leia seu método de cima para baixo como uma narrativa, ele deve fazer sentido
- Aplique uma boa indentação

### Comentários

- Comentários não vão ajudar um código ruim ser melhor interpretado
- Um código que requer comentário precisa ser reescrito
- Não deixe trechos de código comentado

Quando comentar?

- Alertar consequências que podem vir a causar
- Licença, direitos autorais, etc...
- Necessidade de explicar uma regra de negócio interna
- Decisões de design de código
- Utilizar comentários quando os mesmos geram uma documentação do código (Ainda assim, não é tão recomendado)

### Tratamento de erros

- Tratar e prever possíveis exceções é de responsabilidade do desenvolvedor
- Retorne exceptions e não códigos de erro
- Informe o máximo que puder em sua exception
- Se necessário crie exceptions personalizadas para um problema específico
- Não retorne null

[Voltar ao Início](https://github.com/YuriSiman/software-architecture-fundamentals#fundamentos-arquitetura-de-software)  

---

## Design Patterns

Design Patterns são padrões de código para solução de problemas conhecidos. O objetivo não é reinventar a roda, mas sim aplicar uma solução com um bom design de código. O conceito de padrões foi introduzido por 4 desenvolvedores intitulados Gang of Four (GoF) e hoje conta com 23 padrões fundamentais. Atualmente existem mais de 80 padrões conhecidos que são em geral variações dos 23 patterns do GoF.

IMAGEM

Os padrões do GoF estão divididos em 3 famílias:

Família | Descrição
------------ | -------------
Creational Patterns (Criacional) | Fornecem meios de criação de um objeto e de como ele será instanciado
Structural Patterns (Estrutural) | Tratam da composição de objetos por heranças e interfaces para diferentes funcionalidades
Behavioral Patterns (Comportamental) | Tratam das interações e comunicação entre os objetos além da divisão de responsabilidades

[.NET Design Patterns](https://dofactory.com/net/design-patterns)

### Creational Patterns

- Abstract Factory

Cria uma instância de diversas famílias de classes

- Factory Method

Cria uma instância de diversas derivações de classes

- Singleton

Cria uma única instância que será utilizada por os recursos

---

## :vertical_traffic_light: Status do Projeto

:construction: Projeto sendo implementado :construction:

---

## :thinking: Contribuindo

> Para começar...

### Passo 1

* :fork_and_knife: Fork este repositório!

### Passo 2

* :dancers: Clone este repositório para sua máquina local usando `git clone https://github.com/YuriSiman/fundamentals-software-architecture.git`

### Passo 3

* :trident: Crie sua feature branch usando `git checkout -b minha-feature`

### Passo 4

* :white_check_mark: Commit suas mudanças usando `git commit -m "feat: Minha nova feature"`

### Passo 5

* :pushpin: Dê um push usando `git push -u origin minha-feature`

### Passo 6

* :arrows_clockwise: Crie um novo pull request

Depois que seu pull request for mesclado, você pode excluir sua feature branch  

> Caso tenha dúvidas, confira este guia de como [contribuir no GitHub](https://github.com/firstcontributions/first-contributions)  

---

## :speech_balloon: Suporte

> Entre em contato comigo...  

* Me chame pelo [Linkedin](https://www.linkedin.com/in/yurisiman/)  
* Me mande um e-mail [contato@yurisiman.com.br](mailto:contato@yurisiman.com.br)  

[![Github](https://img.shields.io/badge/github-profile-%237159c1?style=for-the-badge&logo=github)](https://github.com/YuriSiman)  
[![Curriculum](https://img.shields.io/badge/site-curriculum-%23563D7C?style=for-the-badge&logo=bootstrap)](https://yurisiman.com.br)  

---

## :pencil: Licença

[![License](https://img.shields.io/badge/license-mit-%23A6CE39?style=for-the-badge&logo=github)](https://github.com/YuriSiman/software-architecture-fundamentals/blob/master/LICENSE)   

---

Code your life...

