---
title: "Universidade X Mundo lá fora"
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
summary: "Há tanta coisa no mundo lá fora... por que não se abrir a isso?"
featured: no
image:
  caption: ''
  focal_point: ''
  preview_only: true
projects: []
---

Recentemente, estive em contato com meu orientador de doutorado para [re] escrever alguns trabalhos que coloquei em um hiato indefinido desde que apresentei minha tese. Não gosto da sensação de ter um trabalho inacabado, então decidi recuperar meu código e rascunhos antigos.

Durante meu mestrado em Astrofísica (2012-2014) usei principalmente Python para escrever o código para a análise de fotos de uma câmera AllSky. Foi muito bom descobrir o quão poderoso é o Python e acompanhar o desenvolvimento de bibliotecas como Pandas e PyRaf (um invólucro em torno do IRAF (Image Reduction and Analysis Facility), o software muito antigo e onipresente para astronomia). Astrônomos são, em geral, ótimos programadores e estão envolvidos no desenvolvimento de software.

No entanto, quando mudei meu tópico de pesquisa para física estatística, entrei em um mundo totalmente novo: código FORTRAN, clusters computacionais e software legado. Era a norma na época: para fazer sua pesquisa você tinha que:

1. Tentar entender o código antigo de seu orientador em uma versão obsoleta da linguagem de programação que ele usava;
2. Tentar construir seu próprio código, mas de uma forma que seu orientador e colegas pudessem entender, isto é, não usando todo aquele software recém lançado que ainda não provou ser realmente útil.

No meu primeiro ano de doutorado, estava lutando para obter uma versão funcional de algum código FORTRAN 77. Tive que entender como simular picos neuronais usando equações de mapa. Envolveu o estudo de diferentes conceitos em sistemas dinâmicos como bifurcação, caos e expoentes de Lyapunov. Logo percebi que não queria escrever uma tese sobre esses assuntos usando FORTRAN 77. Eu queria usar novas ferramentas e métodos. Meu grupo de pesquisa estava começando a usar o MATLAB para alguns cálculos e logo me juntei a eles.

O MATLAB é realmente poderoso. Você pode fazer um ótimo trabalho ao usar matrizes e cálculos numéricos. Se o seu código for lento, você pode transformar facilmente pedaços de código e funções em código C. Plotar é fácil e o resultado é agradável. No entanto, o software em si não é prático, especialmente para alunos e grupos de pesquisa sem recursos. A licença do MATLAB é muito cara e a linguagem não é open source. Muitas pessoas recorrem ao Octave, primo opensource de MATLAB. Voltei para Python.

Mas então eu enfrentei outros problemas: eu era o único usando Python. Se eu quisesse reproduzir alguns códigos de meus colegas, teria que reescrevê-los. E como convencer seu orientador de que você pode realmente FAZER ciência com uma linguagem de programação diferente das que está acostumado?

Este parece ser um problema muito comum na universidade: as pessoas se apegam ao que sabem e isso está comprovado que funciona. Não há muito incentivo para tentar coisas novas. Não há necessidade de realmente otimizar seu código. Você sempre pode * usar o cluster computacional de seu departamento e deixar seu código rodando lá por dias ou até semanas.

Trabalho com ciência de dados há dois anos. É inimaginável esperar mais do que algumas horas para ver o seu código entregar alguns resultados. Se você não usar pacotes ou frameworks atualizados, estará perdendo tempo, dinheiro e, talvez, alguns clientes.

É necessário que o pessoal da universidade comece a se abrir mais para a ideia das novas tecnologias. Muitas linguagens de programação oferecem bibliotecas e ferramentas computacionais poderosas. Julia é uma língua para ficar de olho. Você nem precisa abandonar todo aquele código antigo. Existem bibliotecas maravilhosas que fornecem uma ponte entre diferentes linguagens, como [F2PY](https://numpy.org/doc/stable/f2py/) que permite executar scripts FORTRAN usando uma interface Python, ou Cython, que visa fazer o mesmo, desta vez com C.

Também existem muitos recursos computacionais diferentes disponíveis. Amazon Web Services (AWS), Microsoft Azure e Google Cloud oferecem máquinas virtuais e bancos de dados que são realmente fáceis de usar e configurar. Existem diferentes opções de pagamento e descontos para estudantes e acadêmicos.

No entanto, preciso fazer uma declaração a favor do software de código aberto. Se você é um cientista, muitas vezes não é recomendado depender de recursos pagos para fazer sua pesquisa. A sua bolsa pode ser reduzida ou suspensa, o preço pode subir, etc. Portanto, procure iniciativas abertas e por que não começar a contribuir para elas? Compartilhar conhecimento, trabalho e ferramentas pode melhorar sua rede de contatos e talvez permitir que sua pesquisa seja mais avançada, melhor e mais rápida.

\* _Quando esse cluster está ativo e em execução, o que nem sempre é o caso, é claro._