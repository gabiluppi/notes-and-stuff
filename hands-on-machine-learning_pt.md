# Part 1: The Basics of Machine Learning

### Chapter 1: The Machine Learning Landscape

O primeiro capítulo introduz sobre conceitos de machine learning.

> *É o campo de estudo que possibilita aos computadores a habilidade de aprender sem explicitamente programá-los*
> ***Arthur Samuel, 1959***

> *Alega-se que um programa de computador aprende pela experiência ==E== em relação a algum tipo de tarefa ==T== e alguma medida de desempenho ==P== se o seu desempenho em ==T==, conforme medido por ==P==, melhora com a experiência ==E==.*
> ***Tom Mitchell, 1997***

##### Quando utilizar o aprendizado de máquina?
- A solução de um problema requer muitos ajustes finos ou extensas listas de regras.
- O problema é complexo e não existe uma boa solução utilizando a abordagem tradicional
- O sistema requer uma boa adaptabilidade para novos dados
- Deseja-se entender um problema complexo ou grandes quantidades de dados



#### Tipos de Aprendizado:

---
##### Aprendizado Supervisionado

==O conjunto de treinamento oferecido ao algoritmo inclui as soluções desejadas, chamadas de ***rótulos*** ou ***labels***.==

Os tipos de problemas mais comuns para este tipo de aprendizado são **classificação** (e.g. marcar um e-mail como spam ou ham) e **regressão** (e.g. prever o valor de uma casa baseado nas suas características).

Alguns dos algoritmos mais importantes deste método são:
- K-Nearest Neighbors (KNN)
- Regressão linear
- Regressão logística
- Máquinas de vetores de suporte (SVM)
- Árvores de decisão
- Random Florests
- Redes neurais* (maioria)

---
##### Aprendizado Não Supervisionado

==O conjunto de treinamento não é rotulado.==

Alguns dos problemas e seus algoritmos mais importantes são:
- ==Clusterização==
	- K-Means
	- DBSCAN
	- Análise de cluster hierárquica
- ==Detecção de anomalias e novidades==
	- One-class SVM
	- Floresta de isolamento
- ==Visualização e redução de dimensionalidade==
	- Análise de Componentes Principais
	- Kernel ACP
	- LLE (Locally Linear Embedding)
	- t-SNE (Distributed Stochastic Neighbor Embedding)
- ==Aprendizado de regras por associação==
	- Apriori
	- Eclat

---
##### Aprendizado Semissupervisionado

==O conjunto de treinamento tem apenas uma parte das instâncias rotuladas (geralmente poucas).==

A maior parte dos algoritmos de aprendizado semissupervisionado são combinações de algoritmos supervisionados e não supervisionados:
- Rede neural de crenças profundas (DBN)
- Máquina restritas de Boltzmann (RBM)

---
##### Aprendizado por Reforço

==O sistema de aprendizado (agente) pode assistir o ambiente, selecionar e executar ações e obter recompensas (ou penalidades) em troca.== Ele deve aprender sozinho qual a melhor estratégia (política) para obter o maior número de recompensas. Uma política define o que o agente deve escolher em determinada situação.

---
