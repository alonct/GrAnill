Definiciones de Grupos y Anillos
===

**Author:** *Alonso Oma Alonso*

*Facultad de Matemáticas de la Universidad de Murcia, 2023/2024*

# Índice

- [Definiciones de Grupos y Anillos](#definiciones-de-grupos-y-anillos)
- [Índice](#índice)
- [Tema 1: Anillos](#tema-1-anillos)
  - [Operaciones binarias:](#operaciones-binarias)
  - [Anillos:](#anillos)
  - [Subanillos:](#subanillos)
  - [Homomorfismos de anillos](#homomorfismos-de-anillos)
  - [Ideales y anillo cociente](#ideales-y-anillo-cociente)
- [Tema 2: Divisibilidad en Dominios](#tema-2-divisibilidad-en-dominios)
  - [Cuerpos y dominios; ideales maximales y primos](#cuerpos-y-dominios-ideales-maximales-y-primos)
  - [Divisibilidad](#divisibilidad)
  - [Dominios de factorización única](#dominios-de-factorización-única)
  - [Dominios de ideales principales](#dominios-de-ideales-principales)
  - [Dominios euclideos](#dominios-euclideos)
- [Tema 3: Polinomios](#tema-3-polinomios)
- [Tema 4: Grupos](#tema-4-grupos)
  - [Definiciones y ejemplos](#definiciones-y-ejemplos)
  - [Subgrupos:](#subgrupos)
  - [Subgrupos normales y grupos cociente](#subgrupos-normales-y-grupos-cociente)
  - [Homomorfismos de Grupo Y Teoremas de Isomorfía](#homomorfismos-de-grupo-y-teoremas-de-isomorfía)
  - [El orden de un elemento de un grupo](#el-orden-de-un-elemento-de-un-grupo)
  - [Conjugación y acciones de grupos en conjuntos](#conjugación-y-acciones-de-grupos-en-conjuntos)


# Tema 1: Anillos
## Operaciones binarias:

- _conmutativa_ si $x*y = y*x \ \forall x,\ y\in X$
- _asociativa_ si $x*(y*z) = (x*y)*z \ \forall x,y,z \in X$

Un elemento $x\in X$ se dice que es:

- _neutro_ por la izquierda(derecha) de $X$ con respecto a $*$ si $x*y=y \ \forall y\in X$.
- _cancelable_ por la izquierda (cancelable por la derecha) en $X$ respecto de $*$ si para cada dos elementos distintos $a$ y $b$ de $X$ se verifica $x*a\neq x*b\ (a*x\neq b*x).$
- _simétrico_ si, siendo $e$ un elemento neutro de $X$ con respecto de $*$ y $x$ e $y$ elementos de $X$, diremos que $x$ es simétrico de $y$ por la izquierda y que $y$ es simétrico de $x$ por la derecha con respecto a $*$ si se verifica $x*y=e$.

Tipos de pares $(X,*)$:

- _semigrupo_ si es asociativa;
- _monoide_ si es un semigrupo que tiene un elemento neutro con respecto a $*$;
- _grupo_ si es un monoide y además todo elemento de $X$ es invertible respecto a $*$;
- _grupo abeliano_ si es un grupo y $*$ es conmutativa.

## Anillos:

> Un anillo es una terna $(A,+,\cdot)$ formada por un conjunto no vacío $A$ y dos operaciones $+$ y $\cdot$ en $A$; la primera llamada usualmente suma y la segunda producto o multiplicación, que verifican:
  >1. $(A,+)$ es un grupo abeliano.
  >2. $(A,\cdot)$ es un monoide.
  >3. Distributiva del producto respecto de la suma $a\cdot(b+c) = (a\cdot b) + (a\cdot c)\quad \forall a,b,c\in A$.

Dado un anillo $(A,+,\cdot)$ diremos que un elemento de $A$ es:

- _invertible_ si lo es respecto del producto.
- _regular_ en $A$ si es cancelable con respecto al producto.
- _singular_ en caso contrario.

Llamaremos al conjunto de unidades de $A$ como $A^* = \{x\in A | x\ es\ invertible\}$

## Subanillos:

>Si $A$ es un anillo entonces el conjunto $\mathbb{Z}1 = \{n1 : n ∈ \mathbb{Z}\}$ es un subanillo de $A$ contenido en cualquier otro subanillo de $A$; es decir, $\mathbb{Z}1$ es el menor subanillo de $A$, y se conoce como el _subanillo primo_ de $A$.

## Homomorfismos de anillos

## Ideales y anillo cociente

Un subconjunto $I$ de $A$ es un __ideal__ de $A$ si no es vacío y si, dados $x,y\in I$ y $a\in A$ se verifica que $x+y$ y $ax$ están en $I$.

- Llamaremos ideal __impropio__ de $A$ al propio $A$.
- El ideal __trivial__ será el generado por $0$.
- A cualquier otro ideal lo llamaremos ideal __propio__.

$bA = (b) = \{ba:\ a\in A\}$ es el ideal _principal_ generado por $b$. 
> _Nota:_ $(1) = A,\quad (0) = 0$.
  
Sea $A$ un anillo, y recordemos que si $n\in\mathbb{Z}^+$ escribiremos $n1 = 1+\dots+1$ ($n$ veces). Si existe $n\in\mathbb{Z}^+$ tal que $n1=0$, definimos la característica de $A$ como el menor $n\in\mathbb{Z}^+$ que verifica la igualdad. Si  no existe, diremos que $A$ tiene característica $0$.

>__*<span style="color:orange">Teorema de la correspondencia:</span>*__
>Si $I$ es un ideal de un anillo $A$, las asignaciones $J \mapsto J/I$ y $X \mapsto π^{−1}(X)$ definen aplicaciones >biyecciones (una inversa de la
>otra) que conservan la inclusión entre el conjunto de los ideales de $A$ que contienen a $I$ y el
>conjunto de todos los ideales de $A/I$.

# Tema 2: Divisibilidad en Dominios

## Cuerpos y dominios; ideales maximales y primos

- Un _**cuerpo**_ es un anillo en el que todos los elementos no nulos son invertibles.
- Un _**dominio**_ es un anillo en el que todos los elementos no nulos son regulares.

> **_Observación:_** Cuerpo $\Longrightarrow$ Dominio

Sean $A$ un anillo e $I$ un ideal propio de $A$:
- Se dice que $I$ es __maximal__  si no está contenido en ningún ideal propio (excepto en sí mismo).
- Se dice que $I$ es __primo__ si, $\forall \ a,b\in A$, la relación $ab\in I$ implica $a\in I$ ó $b\in I$.

## Divisibilidad

Sea $A$ un anillo y sean $a,b\in A$. Si existen $c\in A$ tal que $b=ac$ entonces se dice que $a$ __divide__ a $b$ en $A$, o que $a$ es un __divisor__ de $b$ en $A$, o que $b$ es un __múltiplo__ de $a$ en $A$.

Dos elementos $a$ y $b$ de un anillo $A$ se dice que son __asociados__ en $A$ si se dividen mutuamente.

- Diremos que un elemento $a$ del anillo $A$ es __irreducible__ si $0\neq a\in A\backslash A^*$ y la relación $a=bc$ en $A$ implica que $b\in A^*$ ó $c\in A^*$ (y por lo que uno de los dos es asociado de $a$).

- Diremos que $a$ es __primo__ si $0\neq a\in A\backslash A^*$ y la relación $a|bc$ en $A$ implica que $a|b$ ó $a|c$.

Sea $A$ un anillo y sean $S$ un subconjunto de $A$ y $a\in A$:
- $a$ es __máximo común divisor__ (mcd) de $S$ en $A$ si $a$ es divisor de cada elmento de $S$, y múltiplo de cada elemento de $A$ que sea divisor de todos los elementos de $S$.
- $a$ es un __mínimo común múltiplo__ (mcm) de $S$ en $A$ si $a$ múltiplo de cada elemento de $S$, y divisor de cada elemento de $A$ que sea múltiplo de todos los elementos de $S$.

## Dominios de factorización única

Sea $D$ un dominio. Una __factorización en producto de irreducibles__ de un elemento $a$ de $D$ es una expresión del tipo $a=up_1\dots p_n$ con $u\in D^*$ y $p_1,\dots,p_n$ irreducibles de $D$.

Diremos que $D$ es un __dominio de factorización__ o __DF__ si todo elemento no nulo de $D$ admite una factorización en producto de irreducibles.

Dos factorizaciones de $a\in D$ en producto de irreducibles son equivalentes si solo se diferencian en el orden y en asociados.

Diremos que $D$ es __dominio de factorización única (DFU)__ si $\forall 0\neq a\in D$, todas las factorizaciones de a son equivalentes.

> ***Lema:*** Si $D$ es un DFU, entonces todo elemento irreducible de $D$ es primo.

## Dominios de ideales principales

Un __dominio de ideales principales (DIP)__ es un dominio en el que todos los ideales son principales.

## Dominios euclideos

# Tema 3: Polinomios

# Tema 4: Grupos

## Definiciones y ejemplos

>Un grupo es una pareja $(G,\cdot)$ formada por un conjunto no vacío $G$ junto a una operación binaria "$\cdot$", que satisface:
>
>- Asociatividad
>- Existencia de neutro $e\in G$
>- Existencia de inverso: $\forall a\in G\ \exists a^{-1} \ tal \ que\  a\cdot a^{-1} = a^{-1}\cdot a = e$
>
>Si además se verifica la conmutatividad $\forall a,b\in G$ entonces diremos que el grupo es **abeliano** o conmutativo.

De los anteriores axiomas se obtiene de forma más o menos directas las siguientes propiedades:

- Unicidad del neutro
- Unicidad del inverso para cada elemento de $G$
- Todo elemento de $G$ es cancelativo
- $\forall a,b\in G$, las ecuaciones $a\cdot X = b$ y $X\cdot a = b$, tienen una solución única en $G$
- $(a\cdot b)^{-1} = b^{-1}\cdot a^{-1}$

Sean $X$ un conjunto y $S_X$ el conjunto de todas las biyecciones de $X$ en si mismo. Entonces $(S_X, \circ)$ es un grupo, llamado _**grupo simétrico**_ o de las permutaciones de $X$.

Dados dos grupos $(G,\star)$ y $(H, *)$ denotamos el producto directo $G\times H$ a la operación $(g_1,h_1)\cdot(g_2,h_2) = (g_1\star g_2, h_1 * h_2)$.

Dado $n\in \mathbb{N}^+$ definimos $C_n = \{1,a,a^2,\dots,a^{n-1}\}$ formado por $n$ elementos y donde $a$ es un símbolo y la multiplicación viene dado por la siguiente regla: $a^{i}a^j=a^{[i+j]_n}$ donde $[x]_n$ denota el resto de dividir $x$ entre $n$. A este grupo lo llamaremos *__cícllico de orden n__*.

Dado $n\in \mathbb{N}^+$ llamaremos _**grupo diédrico de orden 2n**_ al grupo $D_n = \{1,a,a^2,\dots, a^{n-1},b,ab, a^2b,\dots,a^{n-1}b\}$ cuya multiplicación vendrá dada por la regla $(a^{i_1}b^{j_1})(a^{i_2}b^{j_2}) = a^{[i_1+(-1)^{j_1}i_2]_n}b^{[j_1+j_2]_2}$.

## Subgrupos:

>Sea $G$ un grupo. Un subconjunto $S\subset G$ se dice que es un **subgrupo** si la operación que define la estructura de grupo en $G$ induce también una estructura de grupo en $S$.

Si $G$ es un grupo y $g\in G$, entonces $\lang g\rang = \{g^n:n\in\mathbb{Z}\}$ es un subgrupo de $G$ llamado _**grupo cíclico**_ generado por $g$.

Si $X\subset G$  arbitrario, entonces el conunto formado por todos los elementos de $G$ de la forma $x_1^{n_1}x_2^{n_2}\dots x_m^{n_m}$, con $x_1,\dots,x_m \in X$ y $n_1, \dots, n_m \in \mathbb{Z}$ es un subgrupo de $G$, que resulta ser el menor subgrupo de $G$ que contiene a $X$ y por tanto se llama _**subgrupo generado**_ generado por $X$ y se denota $\lang X \rang$.

Al conjunto $Z(G)= \{g\in G: gx=xg, \forall x\in G\}$ es un subgrupo abeliano de $G$ llamado _**centro**_ de $G$. Más generalmente, sea $x\in G$, entonces $C_G(x)=\{g\in G:gx=xg\}$ es el _**centralizador**_ de $x$ en $G$.
>Obsérvese que $Z(G)$ es la intersección de todos los centralizadores de los elementos de $G$ en $G$.

Sea $G$ un grupo y $H$ un subgrupo de $G$. Se define la siguiente relación binaria en $G$:
$$a\equiv_i b \ mod\ H \Leftrightarrow a^{-1}b\in H\quad\quad(a,b\in G).$$
Se puede comprobar fácilmente que es relación de equivalencia y por tanto define una partición de G en clases de equivalencia. La clase de equivalencia que contiene a $a$ es $aH=\{ah:h\in H\}$ y se llama clase lateral de $a$ módulo $H$ por la izquierda.

Análogamente podemos establecer la relación por la derecha con
$$a\equiv_d b \ mod\ H\Leftrightarrow ab^{-1}\in H\quad\quad(a,b\in G)$$
y las clases de equivalencia dadas por $Ha=\{ha:h\in H\}$.

>El conjunto de las clases laterales por la izquierda de $G$ módulo $H$ se denota por $G/H$ y el de las clases laterales por la derecha $H\backslash G$. Todas las clases laterales tienen el mismo cardinal. $G/H$ y $H\backslash G$ también tienen el mismo cardinal.

> __*<span style="color:orange">Teorema de Lagrange:</span>*__ _Si $G$ es un grupo finito y $H$ es un subgrupo de $G$ entonces $|G| = |H|[G:H]$._

## Subgrupos normales y grupos cociente

Un subgrupo $N$ de un grupo $G$ se dice que es __subgrupo normal__ de $G$ si verífica las condiciones equivalentes de la _Proposición 4.9_ (Codiciones equivalentes a $N\backslash G=G/N$). Esta relación la denotaremos como $N\unlhd G$ (respectivamente $N\lhd G$) para indicar que $N$ es un subgrupo normal (respectivamente normal y propio) de $G$. 

Si $N\unlhd G$, el grupo $G/N$ recién descrito se llama __grupo cociente__ de $G$ módulo $N$.

> __*<span style="color:orange">Teorema de la Correspondencia:</span>*__ Sea $N$ un subgrupo normal de un grupo $G$. La asignación $H\mapsto H/N$ establece una biyección entre el conjunto de los subgrupos de $G$ que contienen a $N$ y el conjunto de los subgrupos de $G/N$.
>
> Además, esta biyección conserva las inclusiones y la normalidad. Es decir, dados dos subgrupos $H$ y $K$ de $G$  que contienen a $N$, se tiene;
>
> 1. $H\subseteq K$ si y sólo si $(H/N)\subseteq (K/N)$
> 2. $H\unlhd G$ si y sólo si $(H/N)\unlhd (G/N)$


## Homomorfismos de Grupo Y Teoremas de Isomorfía

Un _homomorfismo_ del grupo $G$ en el grupo $H$ es una aplicación $f: G\longrightarrow H$ que conserva la operación; es decir, que verifica $f(ab)=f(a)f(b)$ para cualesquiera $a,b\in G$. Si $G=H$ decimos que $f$ es un _endomorfismo_ de $G$.

Si $f$ es un homomorfismo biyectivo, diremos que es un _isomorfismo_. Un _automorfismo_ de $G$ es un isomorfismo de $G$ en $G$.

El _núcleo_ de un homomorfismo $f:G\longrightarrow H$ es 
$$Ker\ f = f^{-1}(1_H)=\{x\in G: f(x) = 1_H\}$$

## El orden de un elemento de un grupo

Sean $G$ un grupo y $a\in G$. Por definición el _**orden**_ de $a$ es el orden del subgrupo $\langle a \rangle$ generado por $a$, y se denota por $|a|$.

Dicho de otra forma, $|a| =$ menor entero no negativo $n$ tal que $a^n = 1$. Y así llegamos a la conclusión de que $a^k=a^l \Leftrightarrow k\equiv l\ mod\ |a|$

> __*<span style="color:lightgreen">Lema:</span>*__ Si $a$ tiene orden finito y $n\in \mathbb{Z}^+$ entoces 
> $$|a^n| = \frac{|a|}{mcd(|a|,n)}$$

> __*<span style="color:orange">Teorema Chino de los Restos para grupos:</span>*__ Si $G$ y $H$ son dos subgrupos cíclicos de órdenes $n$ y $m$, entoces $G\times H$ es cíclico si y sólo si $mcd(n,m) = 1$.
>
> Más generalmente, si $g$ y $h$ son dos elementos de un grupo $G$ de órdenes coprimos $n$ y $m$  y $gh=hg$, entonces $\langle g,h\rangle$ es cíclico de orden $nm$ y $gh$ es un generador.

## Conjugación y acciones de grupos en conjuntos

Sea $G$ un grupo. Si $a,g\in G$, entonces se define el _**conjugado**_ de $g$ por $a$ como $g^{a}=a^{-1}ga$.

Más generalmente, si $X$ es un subconjunto de $G$, entonces el conjugado de $X$ por $a$ es $X^{a}=\{x^{a}:x\in X\}$

Se dice que dos elementos o subconjuntos $x$ y $y$ de $G$ son __*conjugados*__ en $G$ si $x^{a}=y$ para algún $a\in G$.

Sea $\cdot: G \times X \rightarrow X$ una acción por la izquierda de un grupo $G$ en un conjunto $X$. Si $x\in X$ entonces $G\cdot x=\{g\cdot x:g\in G\}$ se llama __*órbita*__ de $x$ y $Estab_G(x) = \{g\in G : g\cdot x = x\}$ se llama __*estabilizador*__ de $x$ en $G$. Obsérvese que las órbitas formas una partición de $G$.