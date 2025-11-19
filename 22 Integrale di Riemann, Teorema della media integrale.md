# 22. Integrale di Riemann, Teorema della media integrale e Teorema fondamentale del calcolo integrale I

Tags: Dimostrazione importante, Integrali
Data lezione: 04/12/2024


Data $f:[a,b]\to\mathbb{R}$ limitata in $[a,b]$, come si può definire e poi calcolare l’area sottesa al suo grafico?

Più in generale l’integrale definisce la somma di infinti contributi infinitesimi e viene impiegato nella definizione e nel calcolo di aree, volumi, spostamenti, lavori,…

# 1. L’integrale di Riemann

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Esistono diverse formulazioni equivalenti dell’integrale di Riemann.


Definiamo in seguito l’integrale di Riemann per $f:[a,b]\to\mathbb{R}$ limitata in $[a,b]$.

Per ogni $n\in \mathbb{N}$ dividiamo $[a,b]$ in n punti di uguale lunghezza $\frac {b-a}n$ tramite i punti 
$x_0= a<x_1<x_2<...<x_{n-1}< x_n=b$ equispaziati e a distanza $\frac {b-a}n$ dal precedente e dal successivo. In ogni intervallo $[x_{k-1}, x_k]$ poi scegliamo arbitrariamente un punto
$t_k^{(n)}\in [x_{k-1},x_k], k = 1,...,n$.

Costruiamo così la **somma di Cauchy - Riemann** definita nel seguente modo.

$$
S_n= \sum_{k=1}^n(x_k-x_{k-1})f(t_k^{(n)})= \frac {b-a} n \sum_{k=1}^nf(t_k^{(n)})
$$

Ad ogni passo della costruzione, in generale, variano sia i punti $x_0,...,x_n$ che realizzano la partizione di $[a,b]$, sia i punti $t_k^{(n)}$. La somma di Cauchy - Riemann dà un valore approssimato di ciò che vogliamo chiamare integrale di Riemann di $f$ in $[a,b]$, ottenuto come somme delle aree di rettangoli $R(x)$, aventi $[x_{k-1},k_k]$ come base e $f(t_k^{(n)})$ come altezza.

$$
S_n= \sum_{k=1}^n(x_k-x_{k-1})f(t_k^{(n)})= \sum_{k=1}^n \operatorname{Area}(R_k)
$$

>Definizione
>**Sia $f:[a,b]\to\mathbb{R}$ limitata in $[a,b]$. Se detta $S_n$ una qualunque successione di somme di Cauchy - Riemann esiste finita tale che $\lim_{n\to\infty}S_n= L\in \mathbb{R}$ ed inoltre tale limite $L\in \mathbb{R}$ non dipende dalla scelta dei punti $t_k^{(n)}$ operata ad ogni passo della costruzione, chiameremo $L= \lim_{n\to\infty}S_n = \int_a^bf(x) \ dx$ integrale di Riemann di $f$ in $[a,b]$.**

>Definizione
>**Se $f:[a,b]\to\mathbb{R}$ limitata in $[a,b]$ è Riemann integrabile in $[a,b]$ e se $f(x)\ge 0$ in $[a,b]$, posto $D= \{(x,y): a\le x\le b, 0\le y\le f(x)\}$, definiamo l’area sottesa al grafico $\operatorname{Area}(D)= \int_a^bf(x) \ dx$.**


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" />**Osservazione**
Se $f:[a,b]\to\mathbb{R}$ limitata in $[a,b]$ è Riemann integrabile in $[a,b]$ e può essere negativa in $[a,b]$ l’area $\int_a^bf(x) \ dx$ è un’area con segno. L’area geometrica della regione di piano compresa tra $x= a,x = b, y = 0$ e il grafico di $f$ è invece data da $\int_a^b|f(x)| \ dx$


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" />**Osservazioni**
- Esistono funzioni limitate che non sono Riemann integrabili e un esempio è la funzione
$f(x) = \begin{cases} 1 , &x\in [0,1]\cap\mathbb Q  \\ 0, &x \in [0,1]\setminus \mathbb Q\end{cases}$
- Se $f:[a,b]\to\mathbb{R}$ non è limitata, essa non è Riemann integrabile

# 2. Classi di funzioni integrabili

>Teorema
> **Se $f:[a,b]\to\mathbb{R}$ è monotona, allora essa è Riemann integrabile in $[a,b]$.**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
$f$ è automaticamente limitata, in quanto se essa è crescente, allora 
$f(a)\le f(x) \le f(b)$, mentre se è decrescente $f(a)\ge f(x) \ge f(b)$.

>Teorema
> **Se $f:[a,b]\to\mathbb{R}$ è continua in $[a,b]$, allora essa è Riemann integrabile in $[a,b]$.**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Dalle ipotesi, per il teorema di Weierstrass, $f$ è automaticamente limitata.

>Teorema
> **Se $a<c<b$ e se $f_1:[a,c]\to\mathbb{R}$ e $f_1:[c,b]\to\mathbb{R}$ sono funzioni Riemann integrabili rispettivamente in $[a,c]$ e $[c,b]$, allora $\forall \alpha \in \mathbb{R}$
$f(x)= \begin{cases} f_1(x) , &x\in [a,c)\\\alpha , &x= c\\f_2(x) ,& x\in (c,b]\end{cases}$ è Riemann integrabile in $[a,b]$.**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Vale un risultato analogo anche nel caso di un numero finito di punti $c_1,...,c_n\in [a,b], \forall n \in \mathbb{N}$.


# 3. Teoremi per integrali definiti
>Teorema
> **Siano $f,g:[a,b]\to\mathbb{R}$ Riemann integrabili, $\alpha,\beta\in \mathbb{R}$. Allora$\alpha f(x) +\beta g(x)$ è Riemann integrabile e vale inoltre che
 $\int_a^b \alpha f(x)+\beta g(x) \ dx = \alpha \int_a^b f(x) \ dx + \beta \int_a^b g(x) \ dx$**
> 

>Teorema
> **Sia $f:[a,b]\to\mathbb{R}$ Riemann integrabile. Sia $\phi :[c,d]\to\mathbb{R}$ è continua e tale che $\operatorname{Im}f\subseteq[c,d]$. Allora $\phi \circ f :[a,b]\to\mathbb{R}$, $\phi\circ f(x) = \phi(f(x))$ è Riemann integrabile.**
> 

>Teorema
> **Se $f$ è Riemann integrabile, allora lo sono anche $|f|, f^2, f^n, e^f, \sin f$**
> 

>Teorema
> **Se $f:[a,b]\to\mathbb{R}$ è Riemann integrabile e $f(x) \ge 0$, allora $\int_a^b f(x) \ dx \ge 0$.**
> 

>Teorema
> **Se $f,g:[a,b]\to\mathbb{R}$ sono Riemann integrabili e $f(x) \ge g(x)$ in $[a,b]$, allora $\int_a^bf(x) \ dx \ge \int_a^bg(x) \ dx$**
> 

>Teorema
> **Se $f:[a,b]\to\mathbb{R}$ è Riemann integrabile, allora 
$|\int_a^b f(x) \ dx| \ge \int_a^b |f(x)| \ dx$**
> 

# 4. Teorema della media integrale

>Teorema della media integrale
> **Sia $f:[a,b]\to\mathbb{R}$ continua in $[a,b]$. Allora $\exists x_0\in[a,b]$ tale che $f(x_0)=\frac 1{b-a}\int_a^bf(x)\ dx$.**
> 

>Definizione: Valor medio
>**Se $f:[a,b]\to\mathbb{R}$ è Riemann integrabile in $[a,b]$, allora $\frac 1{b-a}\int_a^bf(x)\ dx$ si dice valor medio di $f$ in $[a,b]$.**


## 4.1 Dimostrazione

Essendo $f$ continua in $[a,b]$, essa è Riemann integrabile in $[a,b]$. 

Per il Teorema di Weierstrass inoltre essa ammetta massimo e minimo assoluto in $[a,b]$, con $m = \min f$ e $M = \max f$. Ne consegue che $m \le f(x) \le M , \forall x \in [a,b]$.

Poiché $m$  e $M$  sono integrabili, per le monotonie dell’integrale viste nel paragrafo 3 di questo capitolo, possiamo ricavare quanto segue.

$$
\int _a^b m \ dx \le \int _a^bf(x)\ dx \le \int _a^bM\ dx\\m(b-a) \le \int _a^bf(x)\ dx \le M(b-a)\\m\le \frac 1{b-a}\int_a^bf(x)\ dx\le M
$$

Essendo $f$ continua, per il teorema dei valori intermedi $\operatorname{Im}f= [m,M]$. Quindi $\frac 1{b-a}\int_a^bf(x)\ dx\in \operatorname{Im}f\Rightarrow \exists x_0\in [a,b]: f(x_0)=\frac 1{b-a}\int_a^bf(x)\ dx$.

# 5. Teorema fondamentale del calcolo integrale I

>Teorema fondamentale del calcolo integrale I
> **Sia $f:[a,b] \to \mathbb{R}$ Riemann integrabile in $[a,b]$. Supponiamo che $f$ ammetta primitiva $F:[a,b]\to \mathbb{R}$ in $[a,b]$, ossia $F'(x) = f(x)$. 
Allora $\int_a^bf(x) \ dx = F(b) - F(a)= [F(x)]_a^b$.**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Esistono funzioni non Riemann integrabili che non ammettono primitiva, funzioni Riemann integrabili che non ammettono primitiva, funzioni non Riemann integrabili che ammettono primitiva e funzioni Riemann integrabili che ammettono primitiva in $[a,b]$.

In particolare tutte le funzioni continue in $[a,b]$ sono Riemann integrabili e ammettono primitiva in $[a,b]$.


# 6. Regole di integrazione per integrali definiti

## 6.1 Integrazione per parti

>Teorema
> **Siano $f,g:[a,b]\to\mathbb{R}$ funzioni derivabili in $[a,b]$, con $f,g$  Riemann integrabili in $[a,b]$. Allora**
> 
> $$
>   \int_a^b f'(x)g(x) \ dx = f(b)g(b)- f(a)g(a) - \int _a^bf(x)g'(x) \ dx
> $$


## 6.2 Integrazione per sostituzione

>Teorema
> **Siano $f:[a,b]\to\mathbb{R}$ continua,  e $\psi :[\alpha,\beta]\to[a,b]$ derivabile e suriettiva, con $\psi' :[\alpha,\beta]\to[a,b]$ Riemann integrabile in $[a,b]$. Allora**
> 
> 
> $$
> \int_a^b f(x) \ dx= \int_A^B \psi'(t)f(\psi(t)) \ dt , \text{con } x = \psi (t)
> $$
> 
> **dove $A,B\in [\alpha,\beta]$ tali che $\psi(A) = a$  e $\psi (B) = b$.**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Non si richiede che $\psi$ sia invertibile. Nel caso lo fosse, però, $A= \psi^{-1}(a)$  e $B= \psi^{-1}(b)$


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**

È possibile integrare anche funzioni con discontinuità a salto o definite a tratti.

Sia $f:[a,b] \to \mathbb{R}, r_1,...,r_n$ punti in $[a,b]$ tali che $r_0= a< r_1<...<r_n<r_{n+1}= b$ e $f(x) = \begin{cases}f_1(x) , & a\le x < r_1 \\f_2(x) , & r_1< x < r_2\\...\\f_n(x) , & r_{n-1}< x < r_n\\f_{n+1}(x) , & r_n< x \le b\end{cases}$Riemann integrabile in ciascuno dei domini $[r_{i-1};r_i]$.

Allora $f$ è Riemann integrabile in $[a,b]$ e vale che

$$
\int_a^bf(x)\ dx= \sum_{i = 1}^n\int_{r_{i-1}}^{r_i}f_i(x)\ dx
$$
