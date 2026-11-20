# Grafo com Matriz de Adjacência (AEDS III)

Trabalho 1 da disciplina **Algoritmos e Estruturas de Dados III**, do curso de Bacharelado em Sistemas de Informação do IFMG – Campus São João Evangelista.

O programa implementa um grafo (direcionado ou não) usando **matriz de adjacência**, com um menu interativo no terminal.

## Funcionalidades

- Importar um grafo de um arquivo de texto
- Criar um grafo vazio com N vértices
- Exibir a matriz de adjacências
- Consultar se um vértice é adjacente a outro
- Inserir uma aresta (individual ou em conjunto)
- Remover uma aresta
- Editar as coordenadas de um vértice
- Consultar o primeiro adjacente de um vértice
- Consultar o próximo adjacente a partir de um adjacente informado
- Listar todos os adjacentes de um vértice
- Exportar o grafo para um arquivo de texto

## Estrutura do projeto

```
.
├── src/
│   └── trabalho1AEDSIII.cpp
├── exemplos/
│   ├── grafo1.txt
│   ├── grafo2.txt
│   ├── grafo3.txt
│   └── grafo4.txt
├── .gitignore
└── README.md
```

## Como compilar e executar

Requisito: compilador C++ com suporte a C++11 ou superior (g++).

```bash
g++ -std=c++11 -o trabalho1AEDSIII src/trabalho1AEDSIII.cpp
./trabalho1AEDSIII        # Linux/macOS
trabalho1AEDSIII.exe      # Windows
```

## Formato do arquivo de grafo

```
direcionado=nao
10                  <- número de vértices
0 1 1               <- vértice, coordenada X, coordenada Y
1 50 20
...
10                  <- número de arestas
0 1 50              <- origem, destino, peso
0 9 20
...
```

- A primeira linha é `direcionado=sim` ou `direcionado=nao`.
- Peso `0` significa ausência de aresta.
- Em grafos não direcionados, a aresta é gravada uma única vez ao exportar.

## Exemplo de uso

```
-----MENU-----
1 - Importar um grafo de um arquivo de texto.
...
Opção: 1
Qual o nome do arquivo para importação: exemplos/grafo1.txt
```

## Tecnologias

- C++ (STL: `vector`, `fstream`, `iostream`)

## Autor

- Carlos Henrique Lima

## Disciplina

AEDS III – IFMG, Campus São João Evangelista