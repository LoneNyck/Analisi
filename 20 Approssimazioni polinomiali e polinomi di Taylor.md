# 20. Approssimazioni polinomiali e polinomi di Taylor

Tags: Derivate, Dimostrazione importante
Data lezione: 27/11/2024

---

Abbiamo visto che $\sin x = x+o(x), x\to 0$, ma questa approssimazione non sempre è sufficiente. Ad esempio $\lim_{x\to 0}\frac{\sin x-x}{x^3}= \lim_{x\to 0}\frac{o(x)}{x^3}$ che è una forma di indeterminatezza non più risolubile. Applicando il teorema di De L’Hôpital al primo limite possiamo però scoprire il valore del limite che è $-1/6$. Manipolando il limite possiamo quindi scrivere che $\lim_{x\to 0}\frac{\sin x-x+\frac 16x^3}{x^3}=0$, quindi che $\sin x-x+\frac 16x^3 = o(x^3)$, da cui 
$\sin x = x-\frac 16x^3+o(x^3)$. 

![image.png](20%20Approssimazioni%20polinomiali%20e%20polinomi%20di%20Taylo/image.png)

L’approssimazione di $f$ con polinomi di grado al più uno $f(x) = f(x_0)+f'(x_0)(x-x_0)+o(x-x_0)$, $x\to x_0$ realizzata tramite la derivata prima e la notazione di differenziabilità non è sempre sufficiente e occorre trovare polinomi migliori per approssimare $f$ per $x\to x_0$, con grado anche più elevato.

A tale scopo, se $f$ è derivabile in $x_0$ $n$ volte, il candidato più ragionevole è il polinomio di grado al più $n$ che abbia in $x_0$ lo stesso valore di $f$, insieme a tutte le derivate fino a ordine $n$ incluso. Se $P_n(x)$ è tale polinomio, vogliamo che  $P_n^{(k)}(x_0)= f^{(k)}(x_0)$ per $k = 0,...,n$, dove per convenzione $f^{(0)}(x_0) = f(x_0)$.
Dimostreremo che $P_n(x_0)= \sum_{k= 0}^n\frac{f^{(k)}(x_0)}{k!}(x-x_0)^k$.

# 1. Polinomi di Taylor

>Definizione
> **Se $f:(a,b)\to \R$, $x_0\in (a,b)$, $f$ derivabile $n$  volte in $x_0, n\ge 0,$  il polinomio $P_n(x_0)=\sum_{k= 0}^n\frac{f^{(k)}(x_0)}{k!}(x-x_0)^k$ si chiama polinomio di Taylor centrato in $x_0$ di ordine $n$ di $f$. Se $x_0=0$,  si parla anche di polinomio di McLaurin.**


# 2. Teorema di Taylor con il resto in forma di Peano

>Teorema
> **Sia $f:(a,b)\to\R, x_0\in (a,b),f$ derivabile $n$  volte in $x_0,n\ge0$. Allora $f(x) = P_n(x)+o\big((x-x_0)^n\big)=\sum_{k= 0}^n\frac{f^{(k)}(x_0)}{k!}(x-x_0)^k+o\big((x-x_0)^n\big)$, cioè $\lim_{x\to x_0}\frac{f(x)-P_n(x)}{(x-x_0)^n}=0$**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazioni**

- $P_n(x)$ ha grado al più $n$, ma potrebbe aver grado inferiore se $f^{(n)}(x_0)=0$;
- Se $n = 1$, $P_1(x)= f(x_0)+f'(x_0)(x-x_0)$ che è proprio l’espressione della retta tangente ad un punto;
- Si può dimostrare mediante il cambio di variabile che la **derivata del polinomio di Taylor di ordine $n$ di $f$ è il polinomio di Taylor di ordine $n-1$ di $f'$.**
- Esiste al più un polinomio $q(x)$ di grado al più $n$ tale che $\lim_{x\to x_0}\frac{f(x)-q(x)}{(x-x_0)^n}=0$, cioè tale che $f(x) = q(x) + o((x-x_0)^n)$, $x\to x_0$. Se $f$ è derivabile $n$ volte in $x_0$, ne esiste uno ed è proprio il polinomio di Taylor.

## 2.1 Dimostrazione

Dimostriamo il teorema di Taylor per induzione su $n\in \mathbb{N} , n\ge 1$.

1. $P_1(x)$. 
Se $f$ è derivabile 1 volta in $x_0\in (a,b)\Rightarrow$
$f(x_0)+f'(x_0)(x-x_0)+o(x-x_0),$ cioè $f$ è differenziabile in $x_0$. Ciò è vero in quanto sappiamo che $f$ derivabile $\Leftrightarrow$  $f$ differenziabile.
2. $P_{(n-1)}(x)\Rightarrow P_{(n)}(x)$. 
Se $f$ è derivabile n - 1 volte in $x_0, n\ge2$, vale che $\lim_{x\to x_0}\frac{f(x) -\sum_{j= 0}^{n-1}\frac{f^{(j)}(x_0)}{j!}(x-x_0)^j}{(x-x_0)^{n-1}}=0$ come ipotesi di induzione.
    
    Se $f$ è derivabile n volte in $x_0$, $n\ge 2$, $\lim_{x\to x_0}\frac{f(x) -\sum_{k= 0}^n\frac{f^{(k)}(x_0)}{k!}(x-x_0)^k}{(x-x_0)^{n}}  =\lim_{x\to x_0} \frac{f'(x)-P'_n(x)}{n(x-x_0)^{n-1}}=\lim_{x\to x_0}\frac{f'(x) -\sum_{k= 0}^{n-1}\frac{(f')^{(k)}(x_0)}{k!}(x-x_0)^k}{n(x-x_0)^{n-1}}$.
    
    Per l’ipotesi di induzione vale che  $\lim_{x\to x_0}\frac{f'(x) -\sum_{k= 0}^{n-1}\frac{(f')^{(k)}(x_0)}{k!}(x-x_0)^k}{(x-x_0)^{n-1}}= 0$ 
    $\Rightarrow\lim_{x\to x_0}\frac 0 n = 0$.
    
    Per induzione $P_n$ è vera $\forall n\ge1$.
    

## 2.2 Corollario del Teorema di Taylor

>Corollario
> **Sia $f:(a,b)\to\R$ derivabile n volte in $x_0\in(a,b), n\ge2$ e 
$f'(x_0)=f''(x_0)=...=f^{(n-1)}(x_0)=0$ e $f^{(n)}(x_0)\ne 0$. Allora**
> 
> 1. **se $n$ è dispari, $x_0$ è un flesso;** 
> 2. **se $n$  è pari e $f^{(n)}(x_0)\ge 0$, $x_0$ è un minimo;**
> 3. **se $n$  è pari e $f^{(n)}(x_0)\le 0$, $x_0$ è un massimo.**

---

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Siano $f:(a,b)\to\R$, $x_0\in(a,b)$.
Può accadere che $\exists Q(x)$ di grado al più n tale che $f(x) = Q(x) + o((x-x_0)^n), x \to x_0$, senza che $f$ ammetta n derivate.
L’unica eccezione è il caso $n = 1$, in cui $f$ derivabile $\Leftrightarrow$  $f$ differenziabile.


# 3. Teorema di Taylor-Lagrange
>Teorema
> **Sia $f:[a,b]\to\R, x_0\in [a,b],f$ derivabile $n +1$ volte in $[a,b]$. Allora $\forall x \in [a,b]\exists c$ compreso tra $x$  e $x_0$ tale che 
$f(x) = P_n(x)+\frac{f^{(n+1)}(c)}{(n+1)!}(x-x_0)^{n+1} = \sum_{k= 0}^n\frac{f^{(k)}(x_0)}{k!}(x-x_0)^k+\frac{f^{(n+1)}(c)}{(n+1)!}(x-x_0)^{n+1}$.**
> 

Questa formula prende il nome di **formula di Taylor centrata in $x_0$ di ordine $n$ con resto di Lagrange.**

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Per $n=0$, il teorema appena visto è - essenzialmente - il Teorema del valor medio di Lagrange.

# 4. Serie di Taylor

Se $f:I\subseteq\R\to\R, I$ intervallo, $f$ derivabile infinite volte in $I$, $x,x_0\in I$, allora $\forall n\in \mathbb{N}$ possiamo scrivere il polinomio di Taylor $P_n(x)$ di ordine n centrato in $x_0$. Passando al limite $n\to\infty$ otteniamo che $\sum_{k= 0}^\infty\frac{f^{(k)}(x_0)}{k!}(x-x_0)^k$.

>Definizione: Serie di Taylor
>**Se $f:I\subseteq\R\to\R, I$ intervallo, $f$ derivabile infinite volte in $x_0$, definiamo $\sum_{k= 0}^\infty\frac{f^{(k)}(x_0)}{k!}(x-x_0)^k$ come serie di Taylor di $f$ centrata in $x_0$.**


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazioni**

- Le somme parziali N-esime della serie di Taylor di $f$ sono il polinomio di Taylor di ordine n di $f$.
- Non è detto che la serie di Taylor di $f$ centrata in $x_0$ converga, per $x\ne x_0$.
- Se la serie di Taylor di $f$ converge in $x\ne x_0$, non è detto che essa converga a $f(x)$

Alcuni esempi di serie di Taylor sono i seguenti.

$$
e^x= \sum\frac 1 {k!}x^k, \forall x \in \R \\
\sin x= \sum \frac{(-1)^k}{(2k+1)!}x^{2k+1}, \forall x \in \R \\
\cos x =\sum \frac{(-1)^k}{(2k)!}x^{2k}, \forall x \in \R \\
\frac 1 {1-x} = \sum x^k, \forall x\in (-1,1)
$$

## 4.1 Serie di Taylor, numeri complessi e Formula di Eulero

>Definizione
>**$\forall z\in \mathbb C$, definiamo $e^z= \sum\frac {x^k} {k!}$.**


Dimostriamo la formula di Eulero $e^{i\theta} = \cos \theta +i\sin \theta$ mediante le serie di Taylor, già vista in [5. Numeri complessi](5%20Numeri%20complessi%2010c34a788515800ea48ac9acd1bbe90a.md).

$$
 e^{i\theta} = \sum\frac {(i\theta)^k} {k!} = \sum\frac {i^k\theta^k} {k!}= \\
= \sum\frac {i^{2k}\theta^{2k}} {2k!} + \sum\frac {i^{2k + 1}\theta^{2k +1}} {(2k+1)!}= \\
=\sum\frac {(-1)^{k}\theta^{2k}} {2k!} +i\sum\frac {(-1)^k\theta^{2k +1}} {(2k+1)!}\\
\cos \theta +i\sin \theta
$$

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
$e^{a+ib}= e^a\cdot e^{ib}= e^a(\cos b+i\sin b)$