---
layout: post
title: Aula 2 - Verossimilhança (e R)
---

Foram apresentadas ideias sobre probabilidades, distribuições de
probabilidades, esperança matemática, verossimilhança.

**_Objetivo: entender o conceito de verossimilhança. Saber como obter estimadores de máxima verossimilhança em situações simples. Ter um primeiro contato com estatística bayesiana._**

_Arquivos para download:_ [Versão completa](/Biometria-de-Marcadores/pdfs/aula2.pdf) e [para impressão](/Biometria-de-Marcadores/pdfs/aula2_imprimir.pdf).


## Referências

[1] A.W. Edwards, Likelihood, expanded, The Johns Hopkins University Press, 1992.

- Clássico texto que explica em detalhes o conceito de verossimilhança (fazendo uma defesa fervorosa de seu uso).

[2] L. Gonick, W. Smith, The Cartoon Guide to Statistics, Harper Perennial, 1993.

- Livro excelente para alunos sem bom embasamento em Estatística e que procuram um texto simples mas com boa profundidade.

[3] J.G. Kalbfleisch, Probability and Statistical Inference, volume 1, Springer-Verlag, 1985.

- Texto para leitura um pouco mais avançada que o item [2].

[4] I.J. Myung, Tutorial on maximum likelihood estimation, Journal Of Mathematical Psychology. 47 (2003) 90-100.

- Não deixe de ler, principalmente se você não tem bom embasamento e/ou nunca leu nada a respeito. A mais importante dentre todas as referências aqui mencionadas para conseguir entender o curso.

﻿[5] D. Sorensen and D. Gianola, Likelihood, Bayesian, and MCMC Methods in Quantitative Genetics, 1st ed., vol. 81, no. 2. New York, USA: Springer-Verlag, 2002, p. 758.

- Leitura mais avançada, recomendada para quem já tem algum conhecimento sobre o assunto.

[6] D. Koller and N. Friedman, Probabilistic Graphical Models, 1st ed. Massachusetts Institute of Technology, 2009, p. 1266.

- Livro muito bom sobre redes bayesianas.

﻿[7] R. A. Fisher, “On the Mathematical Foundations of Theoretical Statistics,” Philosophical Transactions of the Royal Society of London, A, vol. 222, pp. 309-368, 1922.

- O artigo em que R. A. Fisher apresenta o conceito de verossimilhança.


## Exercícios

### Prazo: 23/03/2015, até a meia-noite.

Os exercícios devem ser enviados por email (exceto quando indicado de
forma diferente), conforme apresentado na aula (veja
[aqui](http://augusto-garcia.github.io/Biometria-de-Marcadores-Introduction/#21)).


1) Leia os itens 9.1 e 9.3 do capítulo 9 da referência [3]

----

2) Suponha que uma população proveniente de um retrocruzamento foi
amostrada, sendo genotipados $$n$$ indivíduos com um marcador
codominante. Destes, $$x$$ apresentaram genótipo homozigoto.

  - Qual é a distribuição de probabilidades que pode ser usada para
    estudar a ocorrência de cada um dos genótipos? Justifique
  - Apresente a função de verossimilhança para esse experimento
  - Deduzir o estimador de máxima verossimilhança para o parâmetro
    $$\theta$$

----

3) Imagine que 4 indivíduos foram genotipados na população acima ($$n=4$$). Faça o gráfico da função de verossimilhança e obtenha estimativas de máxima verossimilhança para theta em cada uma das situações abaixo, com base nos gráficos.

  - $$x=0$$
  - $$x=1$$
  - $$x=2$$
  - $$x=3$$
  - $$x=4$$

----

4) Obtenha estimativas de máxima verossimilhança para os casos 2, 3 e
4 acima, usando os estimadores deduzidos anteriormente. Compare com os
valores obtidos a partir dos gráficos. Interprete os resultados.

----

5) Leia o artigo [4] da Bibliografia. No Fórum, dê sua opinião a
respeito do mesmo, dizendo o que entendeu a respeito, apresentando um
breve resumo das principais ideias. Se entendeu tudo, ajude os colegas
com dúvidas, tanto no Fórum como em grupos de estudo. Se ficou com
dúvidas, busque ajuda junto aos colegas com maior embasamento usando o
Fórum. Em outras palavras, participe de alguma forma!

----

# Introdução ao R

Diferentemente do que foi feito em anos anteriores, desta vez o estudo
do R será iniciado de forma individual, sem apresentação prévia pelo
professor. A ideia é que os alunos desenvolvam maior independência.

**_Objetivo: aprender a usar os principais comandos do R, que será o
  principal programa usado durante o curso. ATENÇÃO: antes da próxima
  aula, aproveite para estudar bastante e começar a usar o pacote.
  Após uma ou duas semanas, faremos uso intensivo do programa e
  assumiremos que todos já dominam os principais conceitos
  envolvidos._**

## Referência

﻿[8] N. Matloff, The Art of R Programming, 1st ed. San Francisco, CA:
No Starch Press, Inc., 2011, p. 404.

- O melhor livro de R que conheço para quem tem interesse em
  programação. Fique atento especialmente aos conceitos sobre
  operações vetoriais, que têm enorme importância nesse ambiente.

## Exercícios

### Prazo: 26/03/2015, até a meia-noite.

6) Visite o tutorial
[Introduction to R](http://augusto-garcia.github.io/R-Introduction/).
Procure entender os principais conceitos.

---

7) Instale o [RStudio](http://www.rstudio.com/) e familiarize-se com
sua interface. Compartilhe suas impressões sobre o mesmo no Fórum.
Aproveite para tirar suas dúvidas.

---

8) Leia o Apêndice A e os capítulos de 1 a 3 do texto
"[An Introduction to R](http://cran.r-project.org/doc/manuals/r-release/R-intro.pdf)",
disponível no site do programa. Pratique usando o RStudio. Compartilhe
sua experiência no Fórum.

---

9) Procure no site do R ou na internet algum tutorial, apostila ou
vídeo(s) que apresente(m) uma introdução ao software. Após
ler/assistir o material, divida sua experiência com os colegas usando
o Fórum, recomendando (ou não) o que encontrou. Seu texto deve ter no
mínimo 15 linhas. Se você já for usuário experiente, ajude quem está
começando com dicas, etc. (A ideia aqui é tentar procurar e recomendar
o material mais legal para quem está começando; quando mais didático,
criativo e estimulante, melhor).
