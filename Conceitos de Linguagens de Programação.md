# Conceitos de Linguagens de Programação
_Sebesta, Robert W._
## Capitulo 1 ##

#### 1.1 Razões para estudar ####

- Aumento da capacidade de expressar ideias.
- Embasamento para escolher linguagens adequadas;.
- Aumento na habilidade de aprender novas linguagens.
	-	[Tiobe indice](https://www.tiobe.com/tiobe-index)
- Melhor entendimento da importância da implementação.
- Melhor uso das linguagens já conhecidas.
- Avanço geral da computação.

#### 1.2 Domínios de programação ####

- Aplicações Científicas
	- ALGOL
- Aplicações Empresarias
	- Cobol
- Inteligencia Artificial
	- List, Prolog
- Para Web
	- Java, PHP, Javascript

#### 1.3 Critérios de Avaliação ####
- Legibilidade
	- Simplicidade
	- Ortogonalidade
	- Tipos de dados
	- Projeto de sintaxe
- Facilidade de Escrita
	- Simplicidade
	- Ortogonalidade
	- Tipos de dados
	- Projeto de sintaxe
	- Suporte a abstração
	- Expressividade
- Confiabilidade
	- Simplicidade
	- Ortogonalidade
	- Tipos de dados
	- Projeto de sintaxe
	- Suporte a abstração
	- Expressividade
	- Verificação de tipos
	- Tratamento de exceções
	- Apelidos restritos
	- Legibilidade e facilidade de escrita
- Custo
	- Ensinar novos programadores
	- Escrever programas nesta linguagem
	- Custo de compilação dos programas
	- Custo de execução
	- Otimização
	- Custo de compilação x Velocidade de execução
	- Código em produção tende a ser executado muitas vezes logo é necessário

#### 1.4 Influências no projeto de linguagens ####
- 1.4.1 Arquitetura dos computadores
	A grande maioria das linguagens são projetadas para computadores da arquitetura de von Neumann (fon noiman)
	A execução de um programa em código de máquina nesta arquitetura ocorre em um processo chamado **ciclo de obtenção e execução**  

	**repita** para sempre
	
		obtenha a instrução apontada pelo contador de programa
		
		incremente o contador de programa a fim de que aponte 
		para a próxima instrução
		
		decodifique a instrução
		
		execute a instrução
	**fim repita**

- 1.4.2 Metodologias de projetos de programas
	
	Software passou a ser mais caro que hardware, logo paradigmas novos foram surgindo, como o Orientação a Dados e o Orientação a Objetos com herança, polimorfismo, vinculação dinâmica e etc.

#### 1.5 Categorias ####
- Imperativas
- Funcionais
- Lógias
- Orientadas a Objetos
- Linguagens de _scripting_

#### 1.6 Trade Off no projeto de linguagens

Muitos critérios são conflitantes como por exemplo
	
	- confiabilidade e custo de execução, muitas verificações , como Java faz, pode elevar o tempo de execução de um programa embora isso deixe o programa mais confiável.

	- facilidade de escrita conflita com legibilidade. Muitos operandos torna a linguagem poderosa e muita computação pode ser feita com poucas linhas no entanto a legibilidade será afetada.

#### 1.7 Métodos de implementação ####

A abtração que o sistema operacional fornece fazendo uma ponte entre as instruções de máquina e o nível de abstração superior é representado por computadores virtuais. Esta abstração é importantíssima para o desenvolvimento de programas.

![diagrama](https://bn1302files.storage.live.com/y4mJIZ_4XEgcm7m5Nac7tfqjasLMBFLRES7AA7FRc7zsfVi0cPeMMtVEp9kfkNBn0J3hWR2qY1KVn1vCgXmXV_wogsmc-T6aFqIooK69XLyrVZbD30rvcY8wBCiRyu_JPr_2O4yruLjliuCkPCOenAkniJVYq_AsBevjOredv2nojFf-PIkCRmZYLc9U_inE5BDtPDjyV-WC8HkhHEk0OrnDQ/diagrama_01.png?psid=1&width=830&height=627)

- 1.7.1 Compilação
	
	Tradução do código para linguagem de máquina trazendo velocidade na execução.
	
	![compilacao](https://bn1302files.storage.live.com/y4mJel6KmnNQklN4CQa2ByF6tHmw-1YGIqHts4xCYyYiMOTIqqF8GtDvXI3ALEKDalwJW3nGa31rcnL1NrwwOX2BOQkvN80AAMnzRQZLKi3tS47kgIdt-DTRF_nkxZ_3fB0jIvMjRN26pD5tCA42VPjQj28-q1ncPhOPd7v_0oLihvIEzg76ZdCxEMmawKYVMwdm0eni1FVLGFuMYOezJpwoQ/diagrama_02.png?psid=1&width=539&height=603)

	Existe também a figura do _linker_ que faz ligação do código compilado a outros programas que o programa do usuário vai precisar para o funcionamento. Pode ser outros progrmamas de usuário ou até bibliotecas que o código precise.

	**gargalo de von Neumann** é o termo designado a limitação na arquitetura dos computadores onde a execução de uma instrução pelo processador é mais rápida do que a taxa de transferência de uma instrução que está na memória para o processador.

- 1.7.2 Interpretação Pura

	<p style='text-align: justify;'>
	Nessa abordagem o programa é interpretado por outro programa, sem tradução. O interpretador age como uma simulação em software de uma máquina cujo ciclo de obtenção-execução trata de sentenças de programa de alto nível em vez de instruções de máquina. Essa simulação de software fornece uma máquina virtual para a linguagem.
	</p>

	<p style='text-align: justify;'>
	Possui a vantagem de fácil depuração uma vez que o erro pode mostrar o ponto exato do código onde o erro está ocorrendo mas possui a desvantagem de ser de 10 a 100 vezes mais lento do que sistemas compilados, uma vez que a decodificação é mais complexa e ocorre várias vezes ao longo da execução do programa. 
	</p>

	![interpretacao](https://poszcw.bn.files.1drv.com/y4mNgJToBnFsZFeNRq6xdDG-_yu89cWCYmPVXifMBZcD0RHSG7EteGI2wd5exUQuibvaPeMDlQaR7-rfexlbS4GHFDLYs8RBk1WomwvNyRMAtlA7z82f-oWe8jli8yyo-8E_hsjJBC7unWJ6Hwrci3W8FrsdBxeuiZbMtt123Nmpr9hkvr4Z6iKwCFNIdWFE3DRFdF0BpzUKgQC6XPfXezbRw?width=552&height=501&cropmode=none)

- 1.7.3 Sistemas de interpretação hibridos

	<p style='text-align: justify;'>
	A maioria utiliza uma abordagem hibrida onde o programa é parcilamente compilado e traduziado para uma linguagem intermediária para em seguida ser traduzido. aumentando a velocidade. 
	</p>

	![implementacao_hibrida](https://xxdyaa.bn.files.1drv.com/y4mVrWjeXudVZjbj3qIL0T_RDN-DAxZKTuibm6E6mg00aEh30UzWh4PMcLKpGmLvSRtEaYKAk5W55O7IuNWdjpNB6T58AoSiA0tiXrRwyIKCq57tfcBYGY-OAbe12XOiDd3bdTqBIOOBrTLlswTzsrza7dpZrUtr8ahvta3opHJNz6Ci0jE_rsvYKEJD5eC1s_xH1_TMZOki7IV3LRPhQyXqQ?width=477&height=550&cropmode=none)

- 1.7.4 Pré Processadores

	Processa outro programa antes de ele ser compilado. As instruções de pré-processador sao imbutidas em programas. Em outras palavras, é um programa de expande macros. 
	
	EX:
	
```
#include "myLib.h"
```

- 1.8 Ambientes de programação
IDE's e Editores de texto.


## Capitulo 2 ##
Evolução das principais linguagens de programação.

![evolução](https://iy4mkw.bn.files.1drv.com/y4mA0ZovQhqqPevpj9FnfxRgo8jVUSs_GdJH-0328dk6UQLwGUSTIDiIAnyoRP6neXckIMmOtQO4NHs1Lw4un3KieVZnIa-Gat32mxyVLXQdeYhbzQyynmZvEqrwlNmxU04kqnLff85jdb3vDLYqC2pHq6-QZHWmiY7RnBb9ZvIft5VfUKKIXjh0g8zNJsxrBSr3hiJvOhT9tjODsjXb962rg?width=351&height=416&cropmode=none)


#### Pontos históricos que eu considero relevantes ####

- IBM 704 e FORTRAN
Cálculos utilizando ponto flutuante eram feitos via software, a IBM foi a primeira a apresentar calculos com ponto flutuante via hardware e foi um ponto muito relevante.

- Lisp e a programação funcional
O interesse em IA se intensificou, as grandes áreas que estavam interessadas seram a linguística, a psicologia e a matemática.
	- Linguísita: interessados no processamento da linguagem.
	- Psicologia: modelos de armazenamentos e recuperação de informações
	- Matemática: Mecanizar processos inteligentes, como prova de teoremas.




