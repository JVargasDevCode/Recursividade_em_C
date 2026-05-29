# Atividade Avaliativa 1 — Recursividade em C

## Descrição

Este projeto foi desenvolvido para a disciplina de Estruturas de Dados e tem como objetivo aplicar conceitos fundamentais de recursividade utilizando a linguagem C.

A atividade aborda diferentes problemas clássicos da computação, explorando tanto soluções recursivas simples quanto versões otimizadas utilizando técnicas como memoização e alocação dinâmica de memória.

---

# Integrantes

- Adryan
- Bruna
- Davi
- Julio
- Natália
- Pedro Woruby

Professor: Goku

---

# Exercícios Desenvolvidos

## 1. Fibonacci Recursivo (Versão Ingênua)

Implementação da sequência de Fibonacci utilizando recursividade simples, sem qualquer otimização.

O programa:
- Recebe um valor `n`
- Calcula o termo correspondente da sequência
- Conta e exibe a quantidade total de chamadas recursivas realizadas

### Caso Base
Quando `n` é igual a `0` ou `1`.

### Redução do Problema
Cada chamada reduz o problema para:
- `fib(n - 1)`
- `fib(n - 2)`

---

## 2. Fibonacci Recursivo com Memoização

Reimplementação do problema anterior utilizando memoização e alocação dinâmica de memória.

O programa:
- Mantém a abordagem recursiva
- Armazena resultados já calculados em memória
- Evita cálculos repetidos
- Compara a quantidade de chamadas com a versão ingênua

### Caso Base
Quando `n` é igual a `0` ou `1`.

### Redução do Problema
Cada chamada continua reduzindo para:
- `fib(n - 1)`
- `fib(n - 2)`

Porém, valores já calculados são reutilizados.

---

## 3. Torres de Hanoi

Implementação recursiva do problema clássico das Torres de Hanoi.

O programa:
- Recebe a quantidade de discos
- Lista todos os movimentos necessários
- Exibe o número total de movimentos realizados

### Caso Base
Mover apenas um disco diretamente para a torre destino.

### Redução do Problema
O problema é reduzido para:
1. Mover `n-1` discos
2. Mover o maior disco
3. Mover novamente `n-1` discos

---

# Tecnologias Utilizadas

- Linguagem C
- Compilador GCC
- Recursividade
- Alocação dinâmica de memória

---

# Restrições Seguidas

- Uso obrigatório de funções recursivas
- Não utilização de variáveis globais
- Não utilização de bibliotecas prontas para resolução direta
- Uso de alocação dinâmica na memoização
- Caso base explícito em todas as soluções

---

# Objetivo Acadêmico

A atividade busca reforçar conceitos importantes relacionados a:
- Recursividade
- Complexidade computacional
- Otimização de algoritmos
- Uso de memória dinâmica
- Divisão e conquista

---

# Compilação

Exemplo utilizando GCC:

```bash
gcc main.c -o programa

Execução:

./programa
