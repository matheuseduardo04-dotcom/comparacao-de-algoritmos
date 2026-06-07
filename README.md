# Comparação: Bubble Sort e Insertion Sort

Projeto simples em Python para estudar e comparar dois algoritmos clássicos de ordenação: **Bubble Sort** e **Insertion Sort**.

O objetivo é entender como cada algoritmo organiza uma lista, quais são suas diferenças e em quais situações um pode se comportar melhor que o outro.

## Estrutura do projeto

```text
sort-comparacao/
├── bubble_sort.py
├── insertion_sort.py
├── comparacao.html
└── README.md
```

## Arquivos

### `bubble_sort.py`

Implementa o algoritmo Bubble Sort.

Esse algoritmo percorre a lista comparando elementos vizinhos. Quando dois elementos estão fora de ordem, eles são trocados de posição. O processo se repete até que a lista esteja ordenada.

No código deste projeto, o Bubble Sort possui uma otimização: se nenhuma troca acontecer durante uma passada, o algoritmo para antes do final, pois a lista já está ordenada.

### `insertion_sort.py`

Implementa o algoritmo Insertion Sort.

Esse algoritmo percorre a lista da esquerda para a direita, pegando um elemento por vez e inserindo-o na posição correta em relação aos elementos anteriores.

Ele costuma funcionar bem quando a lista já está quase ordenada.

### `comparacao.html`

Arquivo reservado para uma possível visualização ou comparação em página HTML.

## Comparação entre os algoritmos

| Característica | Bubble Sort | Insertion Sort |
| --- | --- | --- |
| Ideia principal | Trocar elementos vizinhos fora de ordem | Inserir cada elemento na posição correta |
| Melhor caso | `O(n)` quando a lista já está ordenada | `O(n)` quando a lista já está ordenada |
| Caso médio | `O(n²)` | `O(n²)` |
| Pior caso | `O(n²)` | `O(n²)` |
| Uso de memória | `O(1)` | `O(1)` |
| Indicado para | Estudo inicial de ordenação | Listas pequenas ou quase ordenadas |

## Como executar

Para executar o exemplo do Insertion Sort:

```bash
python3 insertion_sort.py
```

Saída esperada:

```text
[2, 3]
```

Para testar o Bubble Sort pelo terminal:

```bash
python3 -c "from bubble_sort import bubble_sort; print(bubble_sort([5, 3, 1, 4, 2]))"
```

Saída esperada:

```text
[1, 2, 3, 4, 5]
```

## Observação

O arquivo `insertion_sort.py` já possui um exemplo no final:

```python
lista = insertion_sort([3,2])
print(lista)
```

Por isso, ao executar o arquivo, ele imprime o resultado da lista ordenada.

## Conclusão

Os dois algoritmos resolvem o mesmo problema, mas seguem estratégias diferentes.

O **Bubble Sort** é mais simples de visualizar, pois trabalha com trocas entre vizinhos. Já o **Insertion Sort** tende a ser mais eficiente em listas pequenas ou quase ordenadas, porque posiciona cada elemento diretamente no lugar correto.
