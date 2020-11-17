## Bem Vindo a N7

Aqui irei compartilhar algumas coisas que estou estudando para quando eu futuramente precisar de algo especifico, estar tudo aqui documentado.

O foco do blog será compartilhar assuntos como C++, Python, Machine Learning, e 3D, alem de alguns trabalhos do meu curso de pós graduação, com criptografia com SageMath, lógica com a linguagem funcinal Coq, e operações matemáticas com matrizes utilizando Octave.

### Implementação manual de Distâncias (Euclideana, Manhattan, Chebyshev, Camberra e Cosine)
Para realizar a implementação de distâncias na linguagem Python nos é fornecido muitas bibliotecas afim de nos facilitar o trabalho e poupar tempo de reinventar a roda de coisas
que já foram implementas posteriormente e de uma maneira bem otmizada.
Porém no estudo de machine learning se faz necessário aprender afundo como implementar estes cálculos tanto para os entender melhor, quanto para quando se fazer necessário fazer
alguma modificação necessária.
Nesta postagem veremos como implementar algumas das principais métricas de distâncias usadas em machine learning.

```markdown
Syntax highlighted code block

Para implementarmos as distâncias necessitados da linguagem python junto com algumas bibliotecas.
o exemplo apresentado aqui foi implementado em Python 3 (Jupyter Notebook) e as bibliotecas necessárias são:

import pandas as pd #Para realizar a leitura do csv
import scipy.spatial.distance as dist # Para implementarmos as distâncias que jã estão implementadas na nossa biblioteca scipy afim de compararmos os resultados.
import numpy as np # numpy para utilizar alguns métodos matemáticos necessários
import math

# Distancia de Euclides
#Para realizar o calculo da distância Euclideana é necessário fazer o somatório entre a subtração em valor absoluto entre dois pontos distindos (D,D') da nossa base de dados assim tendo o valor mximo da nossa distância.
para implementar precisamos primeiro verificar se o tamanho de x e y, que representam cada um todas as colunas da primeira linha e da segunda respectivamente.
Após isso atribuimos a z o valor de x -z, e entamos fazemos o somatório como representado na imagem da fórmula da Distância Euclideana.

                                                                  def Euclidean(x,y):
                                                                      if x.size != y.size:
                                                                          return (-1)
                                                                      z = x- y
                                                                      diss = math.sqrt((z**2).sum())
                                                                      return diss


## Distancia de Manhattan
 Para realizar o cálculo da distância de Manhattan precisamos seguir a mesma lógica da distância euclideana, porém não precisamos elevar nosso z(x-y) ao quadrado.
                                                                  def Manhattan(x,y):
                                                                    if x.size != y.size:
                                                                        return (-1)
                                                                    z = y-x
                                                                    diss = np.fabs(z).sum()
                                                                    return diss




### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)

```


### C ++
```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![](/Euclidean.png)
```


For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

<div id="mySidenav" class="sidenav">
  <a href="javascript:void(0)" class="closebtn" onclick="closeNav()">&times;</a>
  <a href="#">About</a>
  <a href="#">Services</a>
  <a href="#">Clients</a>
  <a href="#">Contact</a>
</div>

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/NewgateBR/NewgateBR.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
