---
layout: post
title: Aula 3 - Mapas Genéticos I (Segregação Mendeliana)
---

Foram apresentadas ideias sobre testes de hipóteses, p-valores,
problemas de múltiplos testes (Bonferroni, FDR, etc). Em seguida, um
conjunto de dados de uma população de retrocruzamento foi analisado e
discutido.

**_Objetivo: Habilitar os alunos a identificar problemas inerentes à
  realização de múltiplos testes. Discutir problemas com falsos
  positivos. Aprender a testar segregação mendeliana para conjuntos de
  dados de mapeamento genético._**

_Arquivos para download:_ [Versão completa](/Biometria-de-Marcadores/pdfs/aula3.pdf) e [para impressão](/Biometria-de-Marcadores/pdfs/aula3_imprimir.pdf).


## Referências

[1] B.H. Liu, Statistical Genomics - Linkage, Mapping and QTL Analysis, 1 ed., New York, CRC Press, 1998.

- Livro que apresenta vários aspectos do mapeamento genético, dando ênfase nos procedimentos estatísticos. Há discussão sobre testes da segregação mendeliana.

[2] S. Draghici, Data Analysis Tools for DNA Microarrays, Boca Raton, Florida, Chapman and Hall/CRC, 2003.

- Livro escrito em linguagem simples que apresenta os principais métodos estatísticos usados para análise de dados de microarranjos. No capítulo 9 apresenta os problemas dos múltiplos testes, incluindo _Bonferroni_ e _FDR_. Algum cuidado é necessário, já que não há um grande rigor com a terminologia usada em várias partes.


[3] N.C. Oraguzie, E.H. Rikkerink, S.E. Gardiner, Association Mapping in Plants, Springer, 2007.

- No capítulo 7, os autores apresentam uma excelente discussão sobre o problema dos múltiplos testes e o conceito de _p-valor_.


﻿[4] Y. Benjamini, Y. Hochberg, On the Adaptative Control of the False Discovery Rate in Multiple Testing with Independent Statistics, Journal Of Educational And Behavioral Statistics. 25 (2000) 60-83.

[5] Y. Benjamini, Y. Hochberg, Controling the False Discovery Rate: A Practical and Powerful Approach to Multiple Testing, Journal Of The Royal Statistical Society, Series B. 57 (1995) 289-300.

[6] Y. Benjamini, D. Yekutieli, The Control of the False Discovery Rate in Multiple Testing Under Dependency, The Annals Of Statistics. 29 (2001) 1165-1188.

- As referências [4-6] apresentam o conceito de _FDR_ em sua forma original, que motivou toda a discussão sobre controle de falsos positivos.

[7] L. Chen, J.D. Storey, Relaxed significance criteria for linkage analysis., Genetics. 173 (2006) 2371-2381.

- Artigo de fácil leitura que discute de maneira muito interessante as razões pelas quais o _FDR_ não deve ser usado para mapeamento de QTLs em situações comuns (ex: poucos caracteres avaliados)

[8] S. Xu, Quantitative trait locus mapping can benefit from segregation distortion., Genetics. 180 (2008) 2201-2208.

- O título que já diz tudo.

[9] K. Hao, E.E. Schadt, J.D. Storey, Calibrating the performance of SNP arrays for whole-genome association studies., PLoS Genetics. 4 (2008) e1000109.

[10] L. Käll, J.D. Storey, M.J. MacCoss, W.S. Noble, Posterior error probabilities and false discovery rates: two sides of the same coin., Journal Of Proteome Research. 7 (2008) 40-44.

- Artigo de leitura bastante simples que apresenta claramente como
interpretar o significado de FDR, q-valor, etc.

[11] J.T. Leek, J.D. Storey, A general framework for multiple testing dependence., Proc. Natl. Acad. Sci USA. 105 (2008) 18718-23.

- Artigo muito interessante que apresenta alternativas para controle
da dependência entre múltiplos testes de uma forma bastante elegante e
inovadora.

[12] J.D. Storey, The optimal discovery procedure: a new approach to simultaneous significance testing, J. R. Statist. Soc. B. 69 (2007) 347-368.

[13] J.D. Storey, A direct approach to false discovery rates, J. R. Statist. Soc. B. 64 (2002) 479-498.

[14] J.D. Storey, The positive false discovery rate: a bayesian interpretation and the q-value, The Annals Of Statistics. 31 (2003) 2013-2035.

[15] J.D. Storey, J.Y. Dai, J.T. Leek, The optimal discovery procedure for large-scale significance testing, with applications to comparative microarray experiments., Biostatistics (Oxford, England). 8 (2007) 414-432.

[16] J.D. Storey, J.E. Taylor, D. Siegmund, Strong control, conservative point estimation and simultaneous conservative consistency of false discovery rates: a unified approach, J. R. Statist. Soc. B. 66 (2004) 187-205.

[17] Leek, J. T., & Storey, John D. (2011). The Joint Null Criterion for Multiple Hypothesis Tests. Statistical Applications in Genetics and Molecular Biology, 10(1).

- Os artigos [9-17] são alguns dos mais importantes produzidos pelo grupo do John Storey e apresentam em detalhes vários aspectos da moderna discussão sobre múltiplos testes em experimentos genômicos.

[18] J.D. Storey, R. Tibshirani, Statistical significance for genomewide studies. Proc. Natl. Acad. Sci USA. 100 (2003) 9440-9445.

- Na minha opinião, artigo de leitura indispensável para entender os
conceitos de FDR, etc. Fornece novas e influentes ideias sobre o
assunto.

[19] Storey, J D. (2011). False Discovery Rates. In M. Lovic (Ed.), International Encyclopedia of Statistical Science (Vol. 1, pp. 504-508). Springer-Verlag.

- Excelente texto para um conhecimento geral sobre o assunto.

[20] Storey, J D (2011) Interview with Nature Biotechnology: New statistical methods for high-throughput sequencing. Nature Biotechnology 28: 331-333.


## Exercícios

### Prazo: 30/03/2015, até a meia-noite.

Os exercícios devem ser enviados por email (exceto quando indicado de
forma diferente), conforme apresentado na aula (veja
[aqui](http://augusto-garcia.github.io/Biometria-de-Marcadores-Introduction/#21)).

Todos os exercícios devem ser digitados usando o RStudio (RMarkdown).
No caso dos exercícios envolvendo cálculos feitos no R, **não use
nenhum pacote**, apenas o R "básico" (sem carregar pacotes). Caso
tenha problemas, use o Fórum ou comunidade para tirar suas dúvidas.

1) Leia o item [19] e/ou [10] da bibliografia. Explique o que entendeu sobre o(s) artigo(s) escolhido(s) no Fórum (mínimo: 10 linhas). Caso deseje adquirir um conhecimento mais profundo sobre o assunto, leia também os itens [3] e [18].

----

2) Em seu clássico experimento, Mendel (1866) cruzou linhagens de ervilhas diferentes quanto à forma (e outras características), tendo obtido os resultado apresentados na tabela abaixo (população $$F_2$$). Considere cada uma das plantas separadamente e também o total de sementes para fazer os exercícios.

  - Obter estimativas de máxima verossimilhança do parâmetro $$\theta$$ (probabilidade de uma dada semente ser lisa).
  - Testar se esses valores diferem do esperado sob $$H_0$$. Use o R
    para obter os p-valores. (Você já sabe fazer buscas sobre um
    função que faça isso, certo? A distribuição é de qui-quadrado, obviamente.)
  - Caso o gene que controla esse caráter não mostrasse dominância, qual distribuição de probabilidades deveria ser usada para analisar esses dados? Justifique.
  - Mendel realizou esse mesmo tipo de experimento para várias outras características (7 ao todo) e plantas. São esperados falsos positivos nos seus resultados? Justifique.

| Planta| Sementes lisas | Sementes rugosas |
|------:|---------------:|-----------------:|
|  1   |  45 |  12 |
|  2   |  27 |   8 |
|  3   |  24 |   7 |
|  4   |  19 |  10 |
|  5   |  32 |  11 |
|  6   |  26 |   6 |
|  7   |  88 |  24 |
|  8   |  22 |  10 |
|  9   |  28 |   6 |
|  10  |  25 |   7 |
|--------------------------------------------|

----

3) Considere o arquivo de dados abaixo referente a uma população F2 que foi genotipada com um marcador codominante. Os dados fenotípicos ainda não serão analisados.

  - Carregue os dados no R usando o comando

```
read.csv("http://dl.dropbox.com/u/1968009/maize.csv")
```

  - Verifique se todos os locos possuem segregação mendeliana. Utilize alguma correção para múltiplos testes, caso isso seja necessário. Use o R para fazer as análises.
  - Interprete os resultados do ponto de vista genético.

----

4) Em função do seu perfil profissional, escolha um dos tópicos abaixo para fazer uma postagem no Fórum. Uma postagem de 8-10 linhas é suficiente, de preferência com links para referências importantes (se quiser escrever mais, fique à vontade). O desafio é tornar o assunto claro para os colegas da disciplina que não têm familiaridade com o assunto possam entendê-lo. É óbvio que várias postagens serão sobre o mesmo assunto, então procure ser didático e criativo, complementando o que tiver sido postado antes por outros colegas. Leia e faça comentários (quando for o caso) sobre as postagens de colegas com perfil diferente do seu, sempre no intuito de compartilhar conhecimentos e auxiliar quem não está familiarizado com o assunto.

  - Explique como obter populações de RILs para espécies autógamas (ex: soja) e alógamas com linhagens já disponíveis (ex: milho).
  - Explique o que são marcadores moleculares, sem se preocupar tanto com os protocolos, mas sim com os fundamentos das técnicas.
  - Explique o que é genotipagem por sequenciamento (GBS)
  - Explique o que é um p-valor, listando referências da internet que
    ajudam a entender este conceito.
  - Apresente códigos (comentados) no R mostrando como fazer o teste
 de chi-quadrado para segregação mendeliana para os dados usados em
 aula ("mouse data"). Os dados podem ser obtidos no R usando

```
read.csv("http://dl.dropbox.com/u/1968009/mouse.csv")
```

  - Explique como usar o RStudio para criar uma página na internet
    (arquivo html) com um tutorial no R ensinando a fazer o teste de
    qui-quadrado.
