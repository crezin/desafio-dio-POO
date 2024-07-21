# Desafio: Aprendendo na Prática Programação Orientada a Objetos

## Descrição

Este projeto é parte de um desafio co-criado com a plataforma de cursos online Digital Innovation One para aprender e praticar conceitos de Programação Orientada a Objetos (POO) em Java. O objetivo é implementar um sistema de Bootcamp, que inclui cursos, mentorias e desenvolvedores (Devs) que se inscrevem nos Bootcamps, usando os principais pilares da POO: Abstração, Encapsulamento, Herança e Polimorfismo.

## Estrutura do Projeto

### Classes Principais

#### `Bootcamp`
Representa um Bootcamp que contém vários cursos e mentorias. Possui atributos como nome, descrição, data de início, data de fim, desenvolvedores inscritos e conteúdos (cursos e mentorias). Permite a inscrição de desenvolvedores e armazena os conteúdos oferecidos.

#### `Conteudo`
Classe abstrata que serve como base para `Curso` e `Mentoria`. Define atributos comuns como título e descrição, além de um método abstrato para calcular XP. Fornece uma estrutura comum para os diferentes tipos de conteúdo oferecidos no Bootcamp.

#### `Curso`
Representa um curso dentro do Bootcamp. Herda de `Conteudo` e adiciona o atributo carga horária. Implementa o método de cálculo de XP específico para cursos, considerando a carga horária.

#### `Mentoria`
Representa uma mentoria dentro do Bootcamp. Herda de `Conteudo` e adiciona o atributo data. Implementa o método de cálculo de XP específico para mentorias, que é diferente do cálculo para cursos.

#### `Dev`
Representa um desenvolvedor inscrito no Bootcamp. Possui métodos para inscrição em Bootcamps, progressão nos conteúdos e cálculo de XP total acumulado. Armazena os conteúdos em que o desenvolvedor está inscrito e os que já foram concluídos.

### Classe `Main`
A classe `Main` é utilizada para testar o projeto, criando instâncias de `Curso`, `Mentoria`, `Bootcamp` e `Dev`. Simula a inscrição de desenvolvedores em um Bootcamp, a progressão pelos conteúdos e o cálculo do XP acumulado.

## Contribuindo

Este repositório foi criado para fins de estudo, então contribua com ele. Se você encontrou algum problema ou tem sugestões de melhorias, fique à vontade para abrir uma issue ou enviar um pull request.

## Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.
