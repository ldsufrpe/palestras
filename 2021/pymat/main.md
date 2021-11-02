---
theme: gaia
_class: lead
paginate: true
backgroundColor: #000
backgroundImage: url('https://marp.app/assets/hero-background.jpg')
header: PyMat 2021 
# footer: Leon Silva
marp: true
---
<!-- https://marpit.marp.app/ -->
<style>
    :root {
         /* --color-background: #101010; !important; */ 
	 /* --color-foreground: #1b2d4f !important; */ 
    h1, h2, h3,a {
    font-family: IBM Plex Mono;
    
    }
    
}

header,
footer , a, h3 {
color:  #808080;
}
h1,  h2, h4 {
color: #1b2d4f;
}

</style>

![bg right:20% 60%](images/logo_dm.png)
![bg right:25% 85%](images/logo_b2.png)


## O ecossistema Python para matemática computacional
### Leon Silva

leon.silva@ufrpe.br

---
#### Sobre mim
![bg right:30%](https://image.freepik.com/vetores-gratis/silhueta-com-icones-academicos_23-2147501095.jpg)

- Lic. em Matemática (UFRPE)
- Mestre em Matemática (UFC)
- Doutor em Ciência da Computação (UFPE)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![w:220](https://sagectu.com.br/img/elementos_de_computacao_matematica_com_sagemath.jpg)  

---
#### Outline
- Um pouco sobre Python 
- Comparações sobre outros softwares
- Um passeios sobre a sintaxe do Python
- Pacotes para Matemática computacional
- Onde usar Python



---
#### Por que Python?

![bg 20%](https://upload.wikimedia.org/wikipedia/commons/thumb/0/0a/Python.svg/2048px-Python.svg.png)

---

#### Necessidade dos cientistas:
<!-- header: Por que Python? -->
 - Carregar os dados
 - Manipular e processar dados
 - Manipular e operar com expressões algébricas
 - Visualizar dados e resultados
 - Alta qualidade e precisão
 
---

#### Pontos fortes do Python:
![bg 70% right:20%](https://upload.wikimedia.org/wikipedia/commons/thumb/0/0a/Python.svg/2048px-Python.svg.png)
<!-- header: Por que Python? -->
- Não inventou a roda
- Fácil de aprender
- Legível
- Código eficiente
- Multipropósito

---
![bg 70% right:25%](https://upload.wikimedia.org/wikipedia/commons/thumb/1/18/ISO_C%2B%2B_Logo.svg/1200px-ISO_C%2B%2B_Logo.svg.png)
![bg 70% right:25%](https://upload.wikimedia.org/wikipedia/commons/thumb/b/b8/Fortran_logo.svg/120px-Fortran_logo.svg.png)
<!-- header: Comparando com outros softwares -->

#### C, C++, Fortran
- **Prós**
   - Muito rápida. Muito!   
   - Grátis
- **Contra**
   - Sintaxe dolorosa
   - Gerenciamento manual da memória
   - Difíceis para não programadores.
---
![bg 70% right:20%](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1f/Julia_Programming_Language_Logo.svg/120px-Julia_Programming_Language_Logo.svg.png)

#### Linguagem  Julia 
- **Prós**
   -  Rápido e simples
   - Capacidade de integração com Python
- **Contra**
   - Limitado a cálculos numéricos
   - Pouco testado
---
![bg 180% right:18%](https://www.uc.pt/fctuc/dem/Noticias/quantitative/MATLAB.png)
 
 #### Matlab

- **Prós**
  - Muitos algoritmos disponíveis
  - Rápido
  - Editor integrado e agradável
  - Suporte
- **Contra**
  - Linguagem pobre
  - Código fechado 
  - Pago
---
![bg 120% right:25%](http://www.maplesoft.com/images2015/Maple_lg.png)

![bg 120% right:25%](https://content.wolfram.com/uploads/sites/10/2019/04/Thumb_Mathematica12.png)

 #### Maple, Mathematica
- **Prós**
   - Especializados em computação algébrica   
   - Editor próprio e útil
   - Documentação profissional
   - Suporte
- **Contra**   
   - Sintaxe pobre e confusa 
   - Código fechado 
   - Não é grátis
---

![bg 60% right:20%](https://upload.wikimedia.org/wikipedia/commons/thumb/0/0a/Python.svg/2048px-Python.svg.png)
 #### Python
- **Prós**
   - Várias bibliotecas para Matemática Computacional
   - Linguagem poderosa e simples
   - Gratuito e de código aberto
   - Variedade de editores disponíveis
- **Contra**
   - Nem todos os algoritmos estão disponíveis (ainda)
   

---
<!-- header: Ecossistema científico Python -->
![bg 60%](images/ecosystem.jpg)



---
<!-- header: Rápido tutorial -->
#### Um passeio por Python e Matemática
![bg 20% ](https://upload.wikimedia.org/wikipedia/commons/thumb/0/0a/Python.svg/2048px-Python.svg.png)

---
<!-- header: Tutorial -->
![bg 60% right:20%](https://upload.wikimedia.org/wikipedia/commons/thumb/0/0a/Python.svg/2048px-Python.svg.png)
### Matemática
$$\large\sum_{n=0}^{10}3n$$
### Python
 ```python
soma = 0
for n in range(11):
    sum +=3*n
 ```
---
![bg 60% right:20%](https://upload.wikimedia.org/wikipedia/commons/thumb/0/0a/Python.svg/2048px-Python.svg.png)
### Matemática
$$\large\prod_{n=1}^{10}2n$$
### Python
 ```python
produto = 0
for n in range(1, 11):
    sum *=2*n
 ```
 ---

![bg 60% right:20%](https://upload.wikimedia.org/wikipedia/commons/thumb/0/0a/Python.svg/2048px-Python.svg.png)
### Matemática
$$\large A = \{n^2, \forall n \in\mathbb{N}; 20< n< 100 \}$$
### Python
 ```python
a = 20
b = 100
A = [n for n in range(a, b+1)]
 ```
 ---


 ![bg 60% right:20%](https://upload.wikimedia.org/wikipedia/commons/thumb/0/0a/Python.svg/2048px-Python.svg.png)
#### Matemática
- Sequência de Fibonacci
$
 \begin{cases}
    F_0 =  0, F_1=1 \\
    F_n = F_{n-1} + F_{n-2} & \text{para}\; n>1
  \end{cases}
$
#### Python
 ```python
def F(n):
  if n==0:
    return 0
  elif n<=2:
        return 1
return F(n-1) + F(n-2)
 ```
 ---

 ![bg 60% right:20%](https://upload.wikimedia.org/wikipedia/commons/thumb/0/0a/Python.svg/2048px-Python.svg.png)
#### Matemática
- Resolver: $\,\,ax^2 + bx+ c=0$

#### Python
 ```python
x = (b**2)-(4*a*c) 
if x < 0 :
        print ("Raiz negativa nao pode ser extraida.")
else :
    x = math.sqrt(x)
    x1 = (-b + x)/(2*a);  
    x2 = (-b - x)/(2*a)
    print ('x1 = ',x1, '\nx2 = ', x2)
 ```
 ---
<!-- header: Pacote do ecossistema -->
![bg 85% right:25%](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1a/NumPy_logo.svg/1280px-NumPy_logo.svg.png)
 
#### O que é o NumPy?

- Pacote de extensão para Python para matrizes multidimensionais
- Mais perto do hardware (eficiência)
- Projetado para computação científica (conveniência)
- Também conhecido como computação orientada a array

---
<!-- header: NumPy na Nature  -->
![bg 50% ](images/nature.png)

---
<!-- header: Comparação com Python  -->
 ![bg 85% right:25%](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1a/NumPy_logo.svg/1280px-NumPy_logo.svg.png)
#### Python
 ```python
soma = 0
for n in range(11):
    sum +=3*n
 ```

#### NumPy
 ```python
import numpy

soma = numpy.sum(3*numpy.arange(11));
 ```
 ---
<!-- header: Algebra Linear Numérica  -->
![bg 85% right:25%](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1a/NumPy_logo.svg/1280px-NumPy_logo.svg.png)
#### Matemática
- Dada uma matriz $A$ inversível:
   - Computar a inversa, autovetores e resolver o sistema $\small Ax=b$. 

#### NumPy
 ```python
from numpy import linalg

linalg.inv(A)     #inversa de A

linalg.eigvals(A) #autovalores

linalg.solve(A, b) #Resolve Ax=b
 ```
 ---
<!-- header: Numpy: base para o ecossistema -->
![bg 85% right:25%](images/regiao.png)
#### Matemática
- Gerar coordenadas de 81 pontos na região $\small R=[0,5] \times [0,5]$,  distribuidos uniformemente.
#### NumPy
 ```python
 import numpy as np

nx, ny = (9, 9)
x = np.linspace(0, 5, nx)
y = np.linspace(0, 5, ny)

xv, yv = np.meshgrid(x, y)
 ```
---
<!-- header: Pacote do ecossistema -->
![bg 50% right:30%](https://upload.wikimedia.org/wikipedia/commons/thumb/0/01/Created_with_Matplotlib-logo.svg/1200px-Created_with_Matplotlib-logo.svg.png)
### O que é o Matplotlib?
- Muito usado para gráficos 2d
- Fornece dados e figuras de qualidade de publicação
- Exporta figuras para diversos formatos
- Suporta simulações dinâmicas
- Está integrado ao NumPy


---
![bg 80% right:30%](images/plot1.png)
#### Matplotlib: plot $y=\mathrm{sen}{\,x}$ e $y=\cos{x}$
 ```python

# Gráficos 2D

import numpy as np
import matplotlib.pyplot as plt

X = np.linspace(-np.pi, np.pi, 256)
C, S = np.cos(X), np.sin(X)
plt.plot(X, C)
plt.plot(X, S)
plt.show()

```
---
![bg 80% right:30%](images/plot2.png)
#### Matplotlib: plot $\small z= \mathrm{sen}{\left(\sqrt{x^2+ y^2}\right)}$
 ```python
import numpy as np
import matplotlib.pyplot as plt
from mpl_toolkits.mplot3d import Axes3D

fig = plt.figure()
ax = Axes3D(fig)
X = np.arange(-4, 4, 0.25)
Y = np.arange(-4, 4, 0.25)
X, Y = np.meshgrid(X, Y)
R = np.sqrt(X ** 2 + Y ** 2)
Z = np.sin(R)

ax.plot_surface(X, Y, Z, cmap=plt.cm.hot)
plt.show()
```
---
![bg 80% right:30%](images/pizza.png)
#### Matplotlib: Gráfico de Pizza

 ```python
import matplotlib.pyplot as plt

legendas = 'Fatia 1', 'Fatia 2', 'Fatia 3', 'Fatia 4'
porcentagem = [15, 30, 45, 10]
estourar = (0, 0.1, 0, 0)  

fig, ax = plt.subplots()
ax.pie(porcentagem, estourar, legendas, autopct='%1.0f%%')
ax.axis()  
plt.show()
```
---
![bg 60% right:30% ](https://www.fullstackpython.com/img/logos/scipy.png)
#### O que é o Scipy?
- Pacote principal para algoritmos científicos em Python
- Opera com eficiências matrizes do NumPy
- Dedicadas a muitas aplicações científicas
---
![bg 60% right:30% ](https://www.fullstackpython.com/img/logos/scipy.png)
#### Matemática
- Encontrar mínimo da função escalar $f(x)= x^2+ 10\sin{x}, \, 0<x< 10$.
#### SciPy
 ```python
import numpy as np
from scipy import optimize

def f(x):
    return x**2 + 10*np.sin(x)

optimize.minimize(f, x0=0)
```
---
![bg 60% right:30% ](https://www.fullstackpython.com/img/logos/scipy.png)
#### Matemática
- Calcular $\displaystyle\int_1^{10}\frac{\sin{x}}{x}\, dx$
#### SciPy
 ```python
import numpy as np
from scipy.integrate import quadrature


f = lambda x: np.sin(x)/x
quadrature(f, 1, 10)
```
---
![bg 60% right:30% ](https://www.fullstackpython.com/img/logos/scipy.png)
#### Matemática
- Resolver a EDO $\small\begin{cases}
\dfrac{dy}{dt}=2y & 0\leq t\leq 4\\
y(0)=1
\end{cases}$
#### SciPy
 ```python
def calc_derivada(ypos, tempo):
    return -2 * ypos

from scipy.integrate import odeint

t = np.linspace(0, 4, 40)
y = odeint(calc_derivada, y0=1, t)
```
---
![bg 60% right:25% ](https://upload.wikimedia.org/wikipedia/commons/thumb/5/54/Sympy_logo.svg/1200px-Sympy_logo.svg.png)
#### O que é o SymPy?
- Operações algébricas em expressões algébricas
- Operação exatas do Cálculo
- Resolve equações algébricas
- Resolve EDO's
---
![bg 60% right:25% ](https://upload.wikimedia.org/wikipedia/commons/thumb/5/54/Sympy_logo.svg/1200px-Sympy_logo.svg.png)
#### Matemática
- Expandir a expressão $(x+1)^6$
#### SymPy
 ```python
import sympy

x = sympy.symbols("x")

sympy.expand((x+1)**6)
```
---
![bg 60% right:25% ](https://upload.wikimedia.org/wikipedia/commons/thumb/5/54/Sympy_logo.svg/1200px-Sympy_logo.svg.png)
#### Matemática
- $\small \lim_{x\to 0}\frac{\sin{x}}{x}$ 
-   $\small \frac{d}{dx}\left[\sin{x}\right]$
- $\small \int\log{x}\,dx$
#### SymPy
 ```python
 import sympy 
# cálculos exatos
sympy.limit(sympy.sin(x)/x, x,0) #limite

sympy.diff(sympy.sin(x), x) #derivada

sympy.integrate(sympy.log(x), x) #integral
```
---
![bg 60% right:25% ](https://upload.wikimedia.org/wikipedia/commons/thumb/5/54/Sympy_logo.svg/1200px-Sympy_logo.svg.png)
#### Matemática
- Resolver $\small \begin{cases}
x + 5y = 2\\
-3x + 6y = 15
\end{cases}$
#### SymPy
 ```python
import sympy as sym

x, y = sym.symbols('x, y')

sym.solve((x + 5*y-2, -3*x + 6*y-15), (x, y))
```
---
![bg 60% right:25% ](https://upload.wikimedia.org/wikipedia/commons/thumb/5/54/Sympy_logo.svg/1200px-Sympy_logo.svg.png)
#### Matemática
- Resolver a EDO $\small y''+ 9y=0$
#### SymPy
 ```python
from sympy import Function, dsolve, symbols

x = symbols('x')
y = Function('y')

ddy = sympy.diff(y(x), x, x)

dsolve(ddy +9*y(x), y(x))
```
---
![bg 60% right:20%](https://avatars.githubusercontent.com/u/897180?s=200&v=4)
#### O que é o Scikit-image?
- Processamento de imagens
   - Algoritmos:
     - segmentação
     - transformações geométricas
     - manipulação de cor
     - filtros

---
![bg 70% right:25% ](images/logo_dm.png)
#### Processamento
- Lendo arquivos da web (logo DM-\UFRPE)
#### 
 ```python
from skimage import io
import matplotlib.pyplot as plt

url = https://pymat.com.br/assets/images/logos/logo_dm.png

logo_dm = io.imread('url')
plt.imshow(logo_dm)
plt.axis('off')
plt.show()
```
---
![bg 70% right:25% ](images/logo_dm_gray.png)
#### Processamento
- RGB para tons de cinza
#### Scikit-image
 ```python
from skimage import  color 

logo_dm_grayscale = color.rgb2gray(logo_dem)
plt.imshow(logo_dm_grayscale, cmap=plt.cm.gray)
plt.axis('off')
plt.show()
```
---
![bg 70% right:25% ](images/logo_dm_invert.png)
#### Processamento
- Trocar o primeiro fundo com o segundo
#### Scikit-mage
 ```python
from skimage import  filters

# Otsu's method.
val = filters.threshold_otsu(grayscale) 
plt.imshow(grayscale < val, cmap=plt.cm.gray)
plt.axis('off')
plt.show()
```
---
#### Outros pacotes do ecossistema

![bg 90% ](https://chanzuckerberg.com/wp-content/uploads/2020/05/networkx.png)
![bg 80% ](https://upload.wikimedia.org/wikipedia/commons/thumb/0/05/Scikit_learn_logo_small.svg/1200px-Scikit_learn_logo_small.svg.png)
![bg 80% ](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/300px-Pandas_logo.svg.png)
![bg 60% ](https://docs.enthought.com/mayavi/mayavi/_static/mayavi-logo.png)

---

<!-- header: Baseado em python -->
![bg 70% right:35% ](https://images.g2crowd.com/uploads/product/image/social_landscape/social_landscape_b60f5937b391a668da9bf4723bb1ebcb/sagemath.png)

#### SageMath: o Capitão Planeta
- Inclui os pacotes Python:
   - NumPy
   - SciPy
   - SymPy 
   - Matplotlib
   - NetworkX

- Além do:
   - R
   - Maxima,  GAP e outros 
---
<!-- header: PyMat 2021-->
####  E agora?
![bg 25%](https://as2.ftcdn.net/v2/jpg/04/22/66/65/500_F_422666546_nKFTMD4njSGTiVUKH54ZzqnwPUxfxn0a.jpg)

---
<!-- header: Ecossistema Python -->
#### Onde usar o Python e seus ecossistema

![bg 65% ](https://upload.wikimedia.org/wikipedia/en/c/cd/Anaconda_Logo.png)
![bg 50% ](https://colab.research.google.com/img/colab_favicon_256px.png)
![bg 48% ](https://upload.wikimedia.org/wikipedia/en/7/72/CoCalc_Logo.png)


---
<!-- header: Agradecimentos -->
![bg 65% ](images/thanks.png)


