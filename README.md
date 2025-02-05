# Dicionário em C com Lista Encadeada

Este código implementa um dicionário simples usando uma lista encadeada. Cada nó da lista contém uma palavra em português e sua tradução para o inglês. O dicionário permite inserção de palavras, remoção, pesquisa, e outras operações comuns.

## Funcionalidades

1. **Criação da Lista:**
   - A função `cria_lista()` inicializa a lista encadeada como vazia.

2. **Inserção de Palavras:**
   - **Inserir no Início:** A função `inserir_inicio()` adiciona uma nova palavra no início da lista.
   - **Inserir no Final:** A função `inserir_final()` adiciona uma nova palavra ao final da lista.

3. **Remoção de Palavras:**
   - **Remover do Início:** A função `remover_inicio()` remove o primeiro nó da lista.
   - **Remover do Final:** A função `remover_final()` remove o último nó da lista.

4. **Busca de Palavras:**
   - A função `buscar_palavras()` permite buscar uma palavra no dicionário, verificando tanto a tradução de português para inglês quanto de inglês para português.

5. **Tamanho da Lista:**
   - A função `tamanho_lista()` retorna o número de palavras registradas no dicionário.

6. **Limpeza do Dicionário:**
   - A função `liberar()` remove todas as palavras do dicionário e libera a memória alocada.

7. **Exibição do Dicionário:**
   - A função exibe todas as palavras registradas na lista, com suas traduções correspondentes.

## Estrutura de Dados

A estrutura de dados usada é uma lista encadeada, onde cada nó contém as seguintes informações:

```c
typedef struct palavras {
    char PT[30];  // Palavra em português
    char EN[30];  // Tradução em inglês
} Palavras;

typedef struct lista {
    Palavras dados;     // Dados da palavra
    struct lista* prox; // Ponteiro para o próximo nó
} Lista;
```

## Menu de Operações:
```c
Bem-vindo ao dicionário, digite sua opção:
(Por favor, para a boa utilização, digite todas as palavras em minúsculo)
1-Inserir no início
2-Inserir no final
3-Limpar dicionário
4-Buscar palavras
5-Conferir dicionário
6-Remover início
7-Remover final
8-Tamanho
9-Sair
```

## Próximas atualizações:
**Implementar a tradução de um texto inteiro.**
