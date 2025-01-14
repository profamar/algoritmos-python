# Resolvendo algoritmo QuickSort com GitHub Copilot 🚀

Este repositório apresenta uma implementação do algoritmo de ordenação QuickSort em Python, reconhecido por sua eficiência e ampla aplicação devido ao seu desempenho consistente em média. O projeto integra o desafio proposto na aula "Utilizando o GitHub Copilot para Solucionar Algoritmos em Python", parte do curso Formação GitHub Certification oferecido pela DIO.

## Descrição do Algoritmo
O QuickSort é um algoritmo de ordenação por divisão e conquista. Ele funciona escolhendo um elemento como pivô e particionando o array de forma que todos os elementos menores que o pivô fiquem à esquerda, e todos os elementos maiores que o pivô fiquem à direita. O algoritmo então aplica a mesma lógica recursivamente às sublistas geradas.

## Complexidade
- Pior Caso: O(n²) - Ocorre quando o pivô escolhido é o maior ou o menor elemento em cada partição.

- Caso Médio: O(n log n) - Ocorre quando o pivô escolhido divide bem as partições.

- Melhor Caso: O(n log n) - Ocorre quando as partições são sempre igualmente divididas.

## Como Usar
Para usar este algoritmo, você pode clonar este repositório e executar o script Python com a função QuickSort.

## 🛠️ Tecnologias Utilizadas

- **Python 3.9+**: Linguagem principal para a implementação dos algoritmos.
- **Git & GitHub**: Para versionamento e colaboração.
- GitHub Copilot: Assistente de codificação para aumentar a produtividade.
- **Editor de Código**: Visual Studio Code, PyCharm ou qualquer outro de sua preferência.

## Clonando o Repositório
git clone https://github.com/seu-usuario/algoritmos-python.git

## Executando o Script
cd algoritmos-python
python quicksort.py

## Exemplo de Uso
def quicksort(arr):
    if len(arr) <= 1:
        return arr
    pivot = arr[len(arr) // 2]
    left = [x for x in arr if x < pivot]
    middle = [x for x in arr if x == pivot]
    right = [x for x in arr if x > pivot]
    return quicksort(left) + middle + quicksort(right)

# Teste
array = [3, 6, 8, 10, 1, 2, 1]
print(quicksort(array))  # Deve retornar [1, 1, 2, 3, 6, 8, 10]

## Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request.

## Licença
Este projeto está licenciado sob a Licença MIT. Veja o arquivo LICENSE para mais detalhes.

