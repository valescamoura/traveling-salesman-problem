# Problema do Caixeiro viajante

Solução para o Problema do Caixeiro Viajante (*Traveling Salesman Problem*) desenvolvida como atividade para a disciplina de Tópicos em Sistemas de Programação: Modelagem Computacional em 2021/1.

### Objetivo

Desenvolver um algoritmo para encontrar uma solução (não necessariamente ótima) do Problema do Caixeiro Viajante.

Dado um conjunto de cidades 0, 1, ..., n, encontrar uma rota de custo baixo que, partindo da cidade 0, visita todas as cidades (exatamente uma vez cada), e retorna à cidade 0. O custo da rota é a soma das arestas direcionadas escolhidas para a rota. 

Exemplo: se n=3 e a rota escolhida for 0 -> 3 -> 1 -> 2-> 0, então o custo da rota é C = c(0,3) + c(3,1) + c(1,2) + c(2,0), onde c(a,b) é o custo para ir da cidade "a" para a cidade "b". 

### Solução

O problema foi resolvido, inicialmente, com base no método do vizinho mais próximo. Posteriormente, são realizados múltiplos swaps a fim de otimizar a solução.

### Como executar
```
python traveling_salesman.py
```

### Exemplo de entrada

* 6 cidades
```
0 13.5 11.5 7.4 7.7 4.5
15.7 0 5.2 12.1 23.1 20.0
10.1 7.2 0 7.8 14.4 12.1
7.8 11.2 7.1 0 7.2 4.9
9.3 21.0 15.7 9.0 0 6.4
4.7 16.4 12.2 5.5 4.0 0
```