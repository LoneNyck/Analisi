# 4. Potenze, radici, logaritmi e cardinalità

Tags: Insiemi numerici, Operazioni \
Data lezione: 25/09/2024


# 1. Potenze, radici reali e logaritmi

## 1.1  Potenza
> Teorema
> **Sia $y \in \mathbb{R}: y \ge 0, n \in \mathbb{N} , n\ge 1$. 
Allora $\exists! x \in \mathbb{R} : x \ge 0$ e $x^n = y$**
>

Questo teorema segue dal fatto che la funzione $f: (-\infty, +\infty), f(x) = x^n$  è monotona strettamente crescente, continua, con $\lim_{x\to-\infty}f(x) = 0^+$ e $\lim_{x\to\infty}f(x) = +\infty$

## 1.2 Radice reale
> Definizione: Radice
> **$x = \sqrt[n]{y} = y^{1\over n}$.**
> **Il numero reale $x$ siffatto prende il nome di radice reale di $y$**

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazioni**
- $\sqrt{a^2} = |a|, \forall a \in \mathbb{R}$ 
$\sqrt[n]{y} \ge 0, \forall y >0, \forall n\in\mathbb{N}, n>0$
$\sqrt[n]{y^n} = y, \forall y > 0, \forall n\in\mathbb{N}, n>0$
- $\forall a>0\Rightarrow a^0 = 1$ 
$a^m = a\cdot a \cdot a...$ $m$ volte
$a^{1\over n} = \sqrt[n]{a}$
$a^{m\over n} = (a^{m})^{1\over n} = \sqrt[n]{a^m}$, $\forall a\ge0, m, n \in \mathbb{N}, n\neq 0$
- $\forall a \in \mathbb{R}, a > 0, a^{-1} = \frac{1}{a}$
$a^{-{1\over m}}  =(a^{1\over m})^{-1} = {1 \over a^{1 \over m}}$, $\forall a >0, m \in \mathbb{N}, m\neq 0$
</aside>

## 1.3 Definire $a^b, a, b\in \mathbb{R}, a>0$

Si dice che $a^b$ è **ben definito** $\forall a \in \mathbb{R}, a>0$  e $b \in \mathbb{Q}$, ma come si può definire la medesima equazione se $b \in \mathbb{R}$?

Data l’espansione decimale di $b$  possiamo costruire una successione $\pm a^{b_0}, \pm a^{b_0, b_1}, \pm a^{b_0, b_1b_2}, ..., \pm a^{b_0,b_1...b_k}$  con $k \in \mathbb{N}$ ben definita secondo le precedenti definizioni, infatti $b_0,b_1...b_k \in \mathbb{Q}$.  $a^b$ sarà quindi il limite per $k \to +\infty$ della suddetta successione. Si dimostra che $a^b$ può essere anche caratterizzato come $\sup\{ \pm a^{b_0,b_1...b_k} : k \in \mathbb{N}\}$ oppure $\inf\{ \pm a^{b_0,b_1...b_k} : k \in \mathbb{N}\}$ a seconda che la successione sia crescente o decrescente. 

Possiamo quindi concludere che $a^b$ è **ben definito** $\forall a \in \mathbb{R}, a>0$  e $b \in \mathbb{R}$ e anche che 
$a^b > 0$;  di contro, se $a < 0$  e $b \in \mathbb{R}$, $a^b$ può essere definito solo per alcuni valori…

## 1.4 Logaritmo
> Definizione: Logaritmo
> **Dati $y, a \in \mathbb{R}$ con $y > 0, a >0 , a \neq 1$ $\Rightarrow$ $\exists! x \in \mathbb{R}: a^x = y$.**
> **Definiamo quindi il logaritmo $x= \log_ay$ l’unica soluzione dell’equazione $a^x = y$**

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione** 
$a^{\log_a y} = y$ per definizione, $\forall y >0$

# 2. Cardinalità

> Definizione: Cardinalità
>**Dati $A, B$ insiemi, essi si dicono di uguale cardinalità se possono essere messi in corrispondenza biunivoca, ossia $\forall a \in A, \exists! b \in B.$ Nel linguaggio delle funzioni possiamo scrivere $f: A \to B$ deve essere invertibile, quindi deve essere iniettiva e suriettiva, cioè biettiva.**


## 2.1 Cardinalità numerabile
> Definizione: Cardinalità numerabile
> **La cardinalità di $\mathbb{N}$  e di ogni altro insieme che possa essere messo in corrispondenza biunivoca con esso è detta numerabile.**
> 

Segue una serie di **teoremi** sulla cardinalità.

### 2.1.1: $\mathbb{Z}$ è numerabile

Una corrispondenza biunivoca tra $\mathbb{N}$ e $\mathbb{Z}$ può essere la seguente:

$f: \mathbb{Z} \to \mathbb{N}$

$\begin{matrix} \mathbb{Z} & 0 & 1 & -1 & 2 & -2 & ... & n & -n&... \\ \mathbb{N}& 0 & 1 & 2 & 3 & 4 & ... & 2n-1 & 2n&... \end{matrix}$

### 2.1.2 L’insieme degli interi pari (o dispari) è numerabile

Dimostrazione identica al caso precedente.

### 2.1.3 $\mathbb{Q}$ è numerabile

**Punto i.** Si mostra in seguito che $\mathbb{Q}^+$ è numerabile.

In una tabella infinita vengono disposte tutte le frazioni ${m \over n}, m, n \in \mathbb{N}, m, n \neq 0$, dove nella 
*k-esima* riga dispongo ogni frazione tale che $k = m+n$.

$\begin{matrix} 1. & /\\ 2. & 1 \\ 3. & 1\over 2 & 2 \\ 4. & 1\over 3 & 2\over 2 & 3 \over 1 \\\ ... \end{matrix}$

Ciascuna riga contiene un numero finito di elementi ed in particolare la *k-esima* riga contiene $k-1$  elementi. Tutti i numeri $r \in \mathbb{Q}$ compaiono infinite volte nella tabella, in particolare 
$r = {m \over n}$ comparirà ovunque $k  = n+m$.

Costruiamo la corrispondenza biunivoca tra $\mathbb{Q}^+$ e $\mathbb{N}$ contando gli elementi percorrendo la tabella lungo le diagonali inverse, passando alla successiva ogni volta esauriti gli elementi della corrente, saltando inoltre quelli equivalenti a quelli già presi.

$f: \mathbb{N} \to \mathbb{Q}$

$\begin{matrix} \mathbb{N} & 1 & 2 & 3 & 4 & ... \\ \mathbb{Q} & 1 & 1\over2 & 2 & 1\over3 & ... \end{matrix}$

**Punto ii. $\mathbb{Q}^-$**  è necessariamente numerabile potendo essere messo in corrispondenza biunivoca con $\mathbb{Q}^+$, numerabile. 

$f: \mathbb{Q}^+ \to \mathbb{Q}^-$

$f(r) = -r$

**Punto iii. $\mathbb{Q} = \mathbb{Q}^+ \cup \{0\} \cup \mathbb{Q}^-$** è l’unione di insiemi numerabili, che è sempre numerabile. 

**Punto iv**. La corrispondenza biunivoca tra $\mathbb{Q}$ e $\mathbb{N}$ si costruisce in modo simile a quella vista nel 2.1.1.

$\begin{matrix} \mathbb{N}& 0 & 1 & 2 & 3 & 4 & ... & 2n-1 & 2n&...  \\ \mathbb{Q} & 0 & q_1 & -q_1 & q_2 & -q_2 & ... & q_n & -q_n&... \\ \end{matrix}$

## 2.2 Potenza del continuo

> Teorema
> **$\mathbb{R}$ non è numerabile.**

Poiché $\mathbb{R}$ non è numerabile, ma $\mathbb{N} \sub \mathbb{R}$, diremo che $\mathbb{R}$ ha **cardinalità maggiore** di $\mathbb{N}$.

> Definizione: Cardinalità del continuo
>**La cardinalità di $\mathbb{R}$ si chiama potenza del continuo.**

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
$\mathbb{R} = \mathbb{Q} + \mathbb{R}/\mathbb{Q} \Rightarrow \mathbb{R}/\mathbb{Q}$  non è numerabile, ha cardinalità maggiore di $\mathbb{N}$ e si dimostra avere potenza del continuo.

> Teorema
> **$\mathbb{R}$ ha la stessa cardinalità di ogni insieme al suo interno.**


Infatti si può dimostrare ad esempio che:

- $\mathbb{R}$ ha la stessa cardinalità di $(0; +\infty)$

![$f(x) = e^x$](4%20Potenze,%20radici,%20logaritmi%20e%20cardinalit%C3%A0/image.png)

$f(x) = e^x$

- $\mathbb{R}$ ha la stessa cardinalità di $(-{\pi \over 2}; {\pi \over 2})$

![$f(x) = \arctan x$](4%20Potenze,%20radici,%20logaritmi%20e%20cardinalit%C3%A0/image%201.png)

$f(x) = \arctan x$

> Teorema
> **Si dimostra che $\mathbb{R}$  e $\mathbb{C}$ hanno la stessa cardinalità.**
