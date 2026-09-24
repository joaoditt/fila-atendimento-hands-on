README.md<br>
# Descrição:<br>
Este projeto implementa um sistema básico de filas clássicas, circulares e filas de prioridade em Python. Ele permite visualizar as entradas e saídas de clientes, assim como também permite estudar como essas filas ordenam seus dados, sendo por “ordem de chegada” ou por “ordem de prioridade” alguns exemplos.<br><br>


# Tecnologias Utilizadas:

Python 3.x;

Bibliotecas: random, names, heapq;


# Pré requisitos para o funcionamento:

Ter Python 3 instalado no sistema;

Instalar as dependências necessárias:

!pip install names   <=use esse código para instalar a biblioteca 'names'.

# Executando o Projeto:

Copie ou baixe este repositório;

Execute o script principal em seu terminal;


# Estrutura do Código:

Fila, Clientes: Listas que armazenam os dados do cliente, como nome, ordem de chegada e prioridade;

Enqueue: Adiciona dados ao final da lista;

Dequeue: Remove dados do início da fila;

Head: Referente ao início da fila;

Tail: Referente ao final da fila;

Size: Tamanho da fila.


# Respostas:

A ordem de atendimento da fila de prioridade pode ser diferente da fila clássica porque a fila de prioridade organiza os elementos com base em um nível de importância ou urgência, e não apenas pela ordem cronológica de chegada.

Uma fila de prioridade é ideal para situações onde a urgência ou o valor de uma tarefa supera a ordem de chegada. Alguns exemplos sendo:


Triagem de Pronto-Socorro: Pacientes em estado grave (com risco de vida) são atendidos imediatamente, ultrapassando pessoas com sintomas leves que chegaram antes;

Escalonamento de Processos (CPU): O sistema operacional dá prioridade a processos essenciais do sistema (como o movimento do mouse ou áudio) em detrimento de tarefas em segundo plano (como uma atualização de software);

Entregas de Aplicativos: Pedidos de clientes "Premium" ou entregas de alimentos perecíveis/urgentes são roteirizados e despachados com maior prioridade que as entregas padrão.

Algumas vantagens da fila circular em comparação com outras são:


Capacidade de reaproveitamento de memória total, pois em uma fila linear estática, quando um item é removido, o espaço inicial fica vazio e inutilizável. A fila circular reutiliza esses espaços vazios no início do array conforme os elementos da frente são removidos.

Ideal para buffers de dados, como no exemplo de serviços de “streaming” e comunicação de redes, onde dados antigos são continuamente processados e novos dados ocupam seus lugares.

Porém algumas de suas desvantagens se devem pelo fato da fila circular ter tamanho fixo, dificultando ações como a expansão da fila durante o tempo de execução e a verificação de status: diferenciar se a fila está completamente vazia ou totalmente cheia exige lógica adicional ou uma variável de controle de tamanho, pois em ambos os casos o ponteiro do fim pode encostar no ponteiro do início. 


Pode ocorrer três cenários quando houver a inserção de um dado em uma fila circular cheia:

Bloqueio por Fila Cheia (Overflow / Erro): Na implementação clássica e mais segura, o sistema rejeita a nova inserção e impede que dados antigos sejam corrompidos.

Sobrescrita de Dados (Buffer Circular / Ring Buffer): Em sistemas de fluxo contínuo de dados, a fila é configurada para sobrescrever o elemento mais antigo.

Redimensionamento Dinâmico (Dynamic Resizing): Se a fila for projetada para ser flexível, ela se expandirá de tamanho.




Nome dos Integrantes:

João Pedro Santos

Vitor Manoel

Leonardo Silva Dias
