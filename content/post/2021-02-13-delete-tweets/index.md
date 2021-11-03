---
  title: "Apagando tweets de determinado per�odo"
author: Germano Bortolotto
date: '2020-08-02'
slug: academia-outside
categories:
  - academia
- tools
tags:
  - academia
- open source
- tools
- FORTRAN
subtitle: ''
summary: "H� tanta coisa no mundo l� fora... por que n�o se abrir a isso?"
featured: no
image:
  caption: ''
focal_point: ''
preview_only: true
projects: []
---
  
  Hoje vi uma discuss�o no twitter sobre a possibilidade de excluir tweets de um determinado per�odo, n�o todos, n�o necessariamente os mais antigos. Eu obviamente me meti na conversa e pensei que era algo bem f�cil de implementar, ent�o resolvi criar um tutorial b�sico.

O primeiro passo � conseguir as credenciais de acesso da sua conta no Twitter. Acesse o site [https://developer.twitter.com/](https://developer.twitter.com/) e crie um novo app. Escolha um nome qualquer ("deleteTweet123", por exemplo) e anote em um arquivo de texto os valores de API key,  API secret key e Bearer token.
  
  
  Recentemente, estive em contato com meu orientador de doutorado para [re] escrever alguns trabalhos que coloquei em um hiato indefinido desde que apresentei minha tese. N�o gosto da sensa��o de ter um trabalho inacabado, ent�o decidi recuperar meu c�digo e rascunhos antigos.

Durante meu mestrado em Astrof�sica (2012-2014) usei principalmente Python para escrever o c�digo para a an�lise de fotos de uma c�mera AllSky. Foi muito bom descobrir o qu�o poderoso � o Python e acompanhar o desenvolvimento de bibliotecas como Pandas e PyRaf (um inv�lucro em torno do IRAF (Image Reduction and Analysis Facility), o software muito antigo e onipresente para astronomia). Astr�nomos s�o, em geral, �timos programadores e est�o envolvidos no desenvolvimento de software.

No entanto, quando mudei meu t�pico de pesquisa para f�sica estat�stica, entrei em um mundo totalmente novo: c�digo FORTRAN, clusters computacionais e software legado. Era a norma na �poca: para fazer sua pesquisa voc� tinha que:
  
  1. Tentar entender o c�digo antigo de seu orientador em uma vers�o obsoleta da linguagem de programa��o que ele usava;
2. Tentar construir seu pr�prio c�digo, mas de uma forma que seu orientador e colegas pudessem entender, isto �, n�o usando todo aquele software rec�m lan�ado que ainda n�o provou ser realmente �til.

No meu primeiro ano de doutorado, estava lutando para obter uma vers�o funcional de algum c�digo FORTRAN 77. Tive que entender como simular picos neuronais usando equa��es de mapa. Envolveu o estudo de diferentes conceitos em sistemas din�micos como bifurca��o, caos e expoentes de Lyapunov. Logo percebi que n�o queria escrever uma tese sobre esses assuntos usando FORTRAN 77. Eu queria usar novas ferramentas e m�todos. Meu grupo de pesquisa estava come�ando a usar o MATLAB para alguns c�lculos e logo me juntei a eles.

O MATLAB � realmente poderoso. Voc� pode fazer um �timo trabalho ao usar matrizes e c�lculos num�ricos. Se o seu c�digo for lento, voc� pode transformar facilmente peda�os de c�digo e fun��es em c�digo C. Plotar � f�cil e o resultado � agrad�vel. No entanto, o software em si n�o � pr�tico, especialmente para alunos e grupos de pesquisa sem recursos. A licen�a do MATLAB � muito cara e a linguagem n�o � open source. Muitas pessoas recorrem ao Octave, primo opensource de MATLAB. Voltei para Python.

Mas ent�o eu enfrentei outros problemas: eu era o �nico usando Python. Se eu quisesse reproduzir alguns c�digos de meus colegas, teria que reescrev�-los. E como convencer seu orientador de que voc� pode realmente FAZER ci�ncia com uma linguagem de programa��o diferente das que est� acostumado?
  
  Este parece ser um problema muito comum na universidade: as pessoas se apegam ao que sabem e isso est� comprovado que funciona. N�o h� muito incentivo para tentar coisas novas. N�o h� necessidade de realmente otimizar seu c�digo. Voc� sempre pode * usar o cluster computacional de seu departamento e deixar seu c�digo rodando l� por dias ou at� semanas.

Trabalho com ci�ncia de dados h� dois anos. � inimagin�vel esperar mais do que algumas horas para ver o seu c�digo entregar alguns resultados. Se voc� n�o usar pacotes ou frameworks atualizados, estar� perdendo tempo, dinheiro e, talvez, alguns clientes.

� necess�rio que o pessoal da universidade comece a se abrir mais para a ideia das novas tecnologias. Muitas linguagens de programa��o oferecem bibliotecas e ferramentas computacionais poderosas. Julia � uma l�ngua para ficar de olho. Voc� nem precisa abandonar todo aquele c�digo antigo. Existem bibliotecas maravilhosas que fornecem uma ponte entre diferentes linguagens, como [F2PY](https://numpy.org/doc/stable/f2py/) que permite executar scripts FORTRAN usando uma interface Python, ou Cython, que visa fazer o mesmo, desta vez com C.

Tamb�m existem muitos recursos computacionais diferentes dispon�veis. Amazon Web Services (AWS), Microsoft Azure e Google Cloud oferecem m�quinas virtuais e bancos de dados que s�o realmente f�ceis de usar e configurar. Existem diferentes op��es de pagamento e descontos para estudantes e acad�micos.

No entanto, preciso fazer uma declara��o a favor do software de c�digo aberto. Se voc� � um cientista, muitas vezes n�o � recomendado depender de recursos pagos para fazer sua pesquisa. A sua bolsa pode ser reduzida ou suspensa, o pre�o pode subir, etc. Portanto, procure iniciativas abertas e por que n�o come�ar a contribuir para elas? Compartilhar conhecimento, trabalho e ferramentas pode melhorar sua rede de contatos e talvez permitir que sua pesquisa seja mais avan�ada, melhor e mais r�pida.

\* _Quando esse cluster est� ativo e em execu��o, o que nem sempre � o caso, � claro._