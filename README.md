# Screen Match

Screen Match é um projeto em Java que gerencia filmes e séries, calcula o tempo total de visualização e recomendações baseadas em classificações.

## Funcionalidades

- **Gerenciamento de Filmes e Séries**: Criação e manipulação de objetos `Filme` e `Serie` que herdam de `Titulo`.
- **Cálculo de Tempo Total**: A classe `CalculadoraDeTempo` acumula a duração total de filmes e séries.
- **Recomendações**: A classe `FiltroRecomendacao` filtra e recomenda títulos baseados em classificações.
- **Manipulação de Listas**: Uso de `ArrayList` para gerenciar coleções de filmes e séries.
- **Ordenação e Filtragem**: Ordenação de listas e filtragem de objetos baseados em critérios específicos.
- **Encapsulamento e Polimorfismo**: Uso de modificadores de acesso, getters e setters, e polimorfismo com herança e interfaces.

## Tecnologias Utilizadas

- **Java**
- **Java Collections Framework**

## Estrutura do Projeto

### Pacote `calculos`

- **CalculadoraDeTempo**: Acumula a duração total de filmes e séries.
- **Classificavel**: Interface que define o método `getClassificacao`.
- **FiltroRecomendacao**: Filtra e recomenda títulos baseados em classificações.

### Pacote `modelos`

- **Titulo**: Classe base com atributos e métodos comuns para filmes e séries.
- **Filme**: Herda de `Titulo` e implementa `Classificavel`.
- **Serie**: Herda de `Titulo`.
- **Episodio**: Implementa `Classificavel` e representa um episódio de uma série.

### Pacote `principal`

- **Principal**: Classe principal que instancia objetos, calcula tempo total e aplica filtros de recomendação.
- **PrincipalComListas**: Demonstra manipulação de listas, ordenação e filtragem.
