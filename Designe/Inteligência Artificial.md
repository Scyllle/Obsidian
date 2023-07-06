

*Computação Natural* - 
Ideias são obtidas através da observação da natureza. 
- Redes Neurais Artficiais
- Computação evolutiva 
- Sistema imunológicos artificiais

Estudos sobre a vida de organismos artficiais, Vida artificial. 


*Inteligência computacional* - 
''Mundo cientifico ainda estava distante de conhecer por completo a inteligência humana, portanto era muito cedo para criar algum tipo de IA.''

Redes neurais artificiais (RNA), Computação evolutiva. 
Machine Learning (T. Mitchell)
Desenvolver sistemas capazes de aprender 

- Por si mesmos, experiências e comportamentos passados. 
- Interagindo com o ambiente 
- Por meio de entrada de mapas de dados
  
  **Deep learning** técnica de machine learning, utiliza grandes quantidades de dados não estruturados e possibilita a representação hierárquica das camadas de dados.


![[Pasted image 20230615205913.png]]


*Busca sem informação*
Realizada sem informação adicional sobre os estados, além da definição do problema. Gerar novos estados e verificar se um estado objetivo é alcançado ou não.

*Busca em largura*
BFS - Breadth First search 
Nó raiz é verificado antes dos nós filhos do nó raiz.

*Busca em profundidade*
DFS - Depth firts search. Busca-se o nó mais profundo a partir da raiz. A subárvore é visitada por inteiro. 


Busca com custo uniforme
Busca em profundidade limitada
Busca bidirecional


*Busca informada (Heurística)*
Busca de melhor escolha. O caminho de menor custo do estado N ao objetivo.


*Busca gulosa de melhor escolha*
Expande a busca para o nó que seja o mais próximo do estado objetivo considerando apenas o caminho do estado atual ao próximo estado.

*Busca A* (A estrela)*
Função de avaliação f(n)=g(n)+h(n)
g = custo para ir do nó inicial ao nó n 
h = custo estimado para ir no nó n ao nó objetivo.

![[Pasted image 20230615223534.png]]


Aprender a melhorar a busca = *Espaço de estados do nível Meta* 
Cada passo computacional da busca amarzenam-se os erros cometidos paar evitar cometa o mesmo erro.

**Agente baseados em conhecimento**
- KB: Knowledge base
Utilizam uma base de conhecimento. 
Sentaças: Asserção sobre o mundo. 
Sentenças são expressas em uma linguagem de representação do conhecimento. 
Sentença = Axioma, quando não há derivação de outra.

KB é dinâmico. Inserção de novas sentenças pela operação TELL. Busca por uma, ASK.


- Dados, quaisquer sequências númericas que não possuem significado ou relação. 
- Informação, organizados e rotulados.
=
Conhecimento, composição e organização de informações que permitem raciocinio por parte de um ser humano ou máquina.

#Lógica
Linguagem de propósito geral utilizada para descrever fatos em um mundo. Avaliada sempre em verdadeiro ou falso.


## Lógica Proposicional

Sintaxe define setenças atômicas, símbulo preposicional. Palavras que iniciam com letra maiúscula são símbulos preposicionais. Sempre avaliado em verdadeiro ou falso. 
- Sentenças complexas são feitas a partir de mais simples com o uso de conectivos lógicos
![[Pasted image 20230619200419.png]]
![[Pasted image 20230619200637.png]]

## Lógica de primeira ordem

preposicional = Existência de fatos, LPO = Existência de objetos e da relação entre eles.

Formato: P(t_1,....t_n). P é chamado de predicado e tem um ou n argumentos. LPO contém quantificadores, ao saber, Ex (para todo x) e Ax (para qualquer x)
Termos são constantes, se referem a objetos do mundo real.

*Variavel* denotada com o uso de uma letra minúscula, mais do final do alfabeto. Posições de memória que podem ser ocupadas ou instanciadas por valores.

![[Pasted image 20230619201542.png]]


**Engenharia de conhecimento**

BK, tem um processo chamado (). Investiga o domínio do problema, aprende conceitos importantes e define uma representação formal dos objetos e relações entre objetos no domínio.

Etapas: 
1. Identificar a tarefa
2. Agregar o conhecimento relevante, o engenheiro deve ser especialista no assunto/domínio
3. Definir um vocabulário de predicados e constantes
4. Codificar o conhecimento geral do domínio. Axiomas. Verifica se o conhecimento adquirido foi corretamente convertido.
5. Codificar uma descrição da instância específica do problema
6. Formular consultas de interferência para obter respostas
7. Depurar a base do conhecimento.


**Engenharia otonlógica

OPrganiza tudo no mundo em uma hierarquia de categorias. Definidas categorias de objetos, substâncias e medidas, eventos e conhecimento abstratos.
![[Pasted image 20230619202649.png]]

(Wikidata)


Boa parte do raciocinio feito sobre conceitos ocorre no nível de categorias

*Parte de*
Objetos podem ser agruados como parte de uma categoria de objetos. ParteDe(roda, carro), ParteDe(motor,carro). Relação em Objetos compostos.


**Redes semânticas**

São um sistema que permite a visualização gráfica de uma base de conhecimento e algoritimos para a dedução de propriedades de um objeto.

![[Pasted image 20230619203133.png]]



# Sistemas baseados em conhecimento

Dendral - Primeiro sistema de reconhecimnto intensivo bem sucedido

*Heuristc Programming Project (HPP)* - Investigou até que ponto os sistemas baseados em conhecimento seriam úteis em outras areas de conhecimento. 

MYCIN - Detecção de infecções sanguíneas. 

**Sistema é dito especialista quando seu comportamento ou decisões imita o comportamento de um especialista da área de atuação do sistema.

Algoritmo armazena limitado conhecimento em formato de código. Necessitará de mudança em seu código.

![[Pasted image 20230627213641.png]]

 ETAPAS > 
 
 1. Definição de problema
 2. Aquisição do conhecimento 
 3. Representação do conhecimento 
 4. Codificação
 5. Avaliação do SE
 6. Manutenção

Motor de inferência é o cérebro do SE, pois atua sobre a base de conhecimento.
*Progressivo* - A medida que o usuário vai fornecendo evidências do problema, o sistema vai desencadeando o processo de busca na base de conhecimento até encontrar uma resposta para o usuário.
*Regressivo* - O SE escolhe uma resposta hipótese ao problema, e numa busca reversa, verifica se a resposta é plausível.

![[Pasted image 20230627220714.png]]
![[Pasted image 20230627220949.png]]

TOMADA DE DECISÃO

Imitar um especialista na área em que vai atuar. Tomar uma decisão que melhor representa a de um especialista. Optar a decisão com maior probabilidade de acerto.
Redes de decisão.

REC_ESP

VANTAGENS

armaeza conhecimento de um ou mais especialistas e torna disponivel para uma grande quantidade de usuários. Permite que uma boa parte do conhecimento dos profissionais seja perpetuado e fique disponível.


''Um programa de computador aprende pela experiência E, com respeito a algum tipo de tarefa T e perfomance P, se sua perfomance P na tarefa T melhora com a experiência E''



![[Pasted image 20230630214822.png]]

# Aprendizado automático

![[Pasted image 20230630215738.png]]


*Oversampling* = Técnica que consiste em aumentar a quantidade de registros da classe com menor frquência até que a base de dados possua uma quantidade equilibrada entre as classes da variável alvo. 

*Undersampling* =  Técnica que consiste em manter todos os dados da classe com menor frquência e diminuir a quantidade dos que estão com classe de maior frequência, fazendo com que as obvservações no conjunto possuam dados com variável alvo equilibrada.


# Taxonomia do aprendizado automático 

Supervisionado, não supervisionado e semissupervisionado

1. Dados rotulados, indicação da resposta esperada, dada as características de cada exemplo.
2. Dados não tem rotulação.
3. Parte são rotulados e parte não.

- Clássificação: Objetifica-se, dada as caracteristicas de uma instância,definir uma classe dentre um número finito de possibilidades.
- Regressão: Conjunto de classes é infinito. 


- Agrupamento: Indentificar grupos nos exemplos segundo alguma métrica de similaridade dadas as caracteristicas extraídas dos exemplos.
- Detecção de outliers.


Criação de uma árvore de decisão também chamado de *Indução*

![[Pasted image 20230630224243.png]]


![[Pasted image 20230630224320.png]]

*One hot encoding*
Problemas com valores nominais devem ter os valores convertidos devidamente para valores númericos.

*Regressão lienar*
Técnica matemática que visa minimizar o erro de uma equação cuja representação gemométrica se adapte a um conjunto de pontos.
![[Pasted image 20230630225254.png]]

![[Pasted image 20230630225418.png]]


# Não supervisionada

Não se tem a definição ou anotação das classes do problema, mas ainda assim deseja-se aprender algo.

- Associação
- Agrupamento : K-means


# Redes neurais

Deep learning

Composta por uma grande quantidade de neurônios artificais, formalizados matematicamente.
Cada neurônio tem n entradas (xo a xn), e cada entrada é multiplicada por um peso w. Essas entradas ponderadas são somadas e uma função de ativação é aplicada, definindo a saída do reurônio, que será repassada pra outros neurônios.

![[Pasted image 20230630231506.png]]


- Multiplayer perceptrons

Permite tratamento de problemas não lineares. Perceptron trata apenas de problemas lineares, isto é, classes do problema sejam separáveis por um hiperplano no espaço de atrbutos.

- Redes convolucionais
Utilizada tratamento de imagens. 

*Medidas de avaliação de apredizagem*

PRECISÃO
![[Pasted image 20230630232248.png]]

COBERTURA
![[Pasted image 20230630232323.png]]

MEDIDA F
![[Pasted image 20230630232347.png]]

Incerteza: 
# Probabilidade



*Teorema de Bayes*

Descreve a probabilidade de um evento baseado na observação e quantização de conhecimentos anteriores relacionados ao evento. Computa a probabilidade de uma afirmação dado a um conjunto de observações.
![[Pasted image 20230704180926.png]]




