# Sistema de atendimento online do Bradesco em linguagem C

Este trabalho implementa um sistema de atendimento online, no qual os clientes são inseridos em uma fila de prioridade com base na idade, sendo os mais velhos com maior prioridade.

# Funcionalidades

As funcionalidades presentes no código são:

- Leitura das idads: A leitura das idades dos clientes é realizada em um arquivo d texto "clientes.txt".
- Fila de prioridades: Os clientes são alocados em uma fila de prioridade, no qual é ordenada, para garantir que os mais velhos sejam atendidos primeiro.
- Algoritmo de ordenação: foi utilizado o Bubble Sort para fazer a ordenação de ordem decrescente.
- Atendimento: O sistema remove e imprime a idade dos clientes da fila enquanto são atendidos, a fim de garantir que os mais velhos tenham maior prioridade e sejam atendidos primeiro.


# Estrutura

A estrtura é constituída por:

- Fila Duplamente Encadeada: A fila é implementada utilizando uma estrutura de lista duplamente encadeada, com ponteiros para o próximo e o anterior, com o objetivo de verificar as idades dos seus 'vizinhos' priorizando o de maior idade.
- Estrutura do Nó:
  typedef struct No{
    int valor; 
    struct No* ant;
    struct No* prox;
}No;

Sendo a idade dos clientes representada pela variável valor.

- Fila: É composta por dois ponteiros: sendo um para o "início" da fila e o outro para o "fim" da fila.

# Como executar o código:

