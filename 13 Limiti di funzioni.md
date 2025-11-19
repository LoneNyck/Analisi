# 13. Limiti di funzioni

Tags: Funzioni, Limiti

# 1. Intorni e punti di accumulazione

## 1.1 Intorni

>Definizione: Intorno
>**Dato $x_0\in \mathbb{R}$, chiamiamo intorno di $x_0$ un insieme della forma 
$U(x_0) = (x_0 -\epsilon; x_0 + \epsilon), \forall \epsilon > 0$.**
>
>**Chiamiamo intorno di $+\infty$ un insieme della forma 
$U(+\infty) = (M;  +\infty), \forall M \in \mathbb{R}$.**
>
>**Chiamiamo intorno di $-\infty$ un insieme della forma 
$U(-\infty) = (-\infty; M), \forall M \in \mathbb{R}$.**

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazioni**

- $x_0 \in U(x_0), \forall x_0 \in \mathbb{R}, \forall \epsilon > 0$
- $+\infty \notin U(+\infty), \forall M \in \mathbb{R}$
- $-\infty \notin U(-\infty), \forall M \in \mathbb{R}$

## 1.2. Punti di accumulazione

>Definizione: Punto di accumulazione
>**Dati $x_0 \in \overline \mathbb{R}$ e $I \subseteq$ $\mathbb{R}$ insieme, diremo che $x_0$ è punto di accumulazione per $I$ se e solo se ogni intorno di  $x_0$ soddisfa 
$(U(x_0)\cap I) \setminus\{x_0\} \ne \empty$, ossia esistono elementi di $I$ diversi da $x_0$ in ognuno dei suoi intorni. Si noti che $x_0$ può o meno appartenere a $I$.**


Se $I = (1;2)$ o $I = [1;2)$ o $I = (1;2]$ o $I = [1;2]$, allora i punti di accumulazione di $I$ sono $[1;2]$.

Se $I = (3;+\infty)$ o $I = [3;+\infty)$, allora i punti di accumulazione di $I$  sono
$[3;+\infty) \cup \{+\infty\}$.

Se $I = \mathbb{N}$, l’unico punto di accumulazione è $+\infty$.

Se $I = \mathbb{Q}$, i suoi punti di accumulazione sono $\mathbb{R}\cup \{+\infty\} \cup \{-\infty\} = \overline \mathbb{R}$.

# 2. Diverse definizioni di limite

## 2.1 Definizione successionale

>Definizione successionale
**Sia $f: I \subseteq\mathbb{R} \to \mathbb{R}$ e sia >$x_0\in\overline\mathbb{R}$ un punto di accumulazione per $I$ e $\ell \in \overline \mathbb{R}$. Se per ogni successione $x_n$ tale che: i. $x_n \in I \ \forall n \in \mathbb{N}$, ii. $x_n \neq x_0 \ \forall n \in \mathbb{N}$ e iii. $\lim_{n\to\infty}x_n = x_0$ vale che $\lim_{n\to\infty}f(x_n) = \ell$, allora diremo che $\lim_{x\to x_0}f(x) = \ell$.**


Dalla definizione successionale di limite è molto facile **verificare che il limite di una funzione non esista.** Infatti se esistono due successione $x_n$  e $z_n$ che soddisfano i punti i. ii. e iii. della definizione tali che $\lim_{n\to\infty}f(x_n) \neq \lim_{n\to\infty}f(z_n)$ , allora $\nexists\lim_{x\to\infty}f(x)$.

## 2.2 Teorema di unicità del limite
>Teorema di unicità del limite
> **Dati $f: I \subseteq\mathbb{R} \to \mathbb{R}$, $x_0\in\overline\mathbb{R}$ punto di accumulazione di $I$ e $\ell \in \overline \mathbb{R}$, se $\exists\lim_{x\to\infty}f(x) = \ell$, allora tale limite è unico.**
> 

### 2.2.1 Dimostrazione

Supponiamo per assurdo che esistano due limiti $\ell _1$  e $\ell_2 \in \overline \mathbb{R}$, con $\ell_1 \ne \ell_2$ a cui la funzione $f$ tenda. Dai punti i. ii. e iii. della definizione successionale di limite si conclude che $\lim_{n\to\infty}f(x_n) = \ell_1$, $\lim_{n\to\infty}f(x_n) = \ell_2$, ma $\ell_1 \ne \ell_2$ per ipotesi e questo è in contraddizione con il teorema di unicità del limite visto per le successioni [[7. Successioni e introduzione ai limiti](7%20Successioni%20e%20introduzione%20ai%20limiti%2011334a78851580b9b79fcb0887cf2531.md), par. 2.3].

## 2.3 Definizione topologica

>Definizone topologica
>**Sia $f: I \subseteq\mathbb{R} \to \mathbb{R}$ e sia $x_0\in\overline\mathbb{R}$ un punto di accumulazione per $I$ e $\ell \in \overline \mathbb{R}$. Diremo che $\lim_{x\to x_0}f(x) = \ell$ se e solo se per ogni intorno $U(\ell)$ di $\ell$ esiste un intorno $U (x_0)$ di $x_0$ tale che: i.  $x \in U(x_0)$, ii. $x\in U(x_0)\Rightarrow f(x) \in U(\ell)$, iii. $x \neq x_0$.**

Tradotto in linguaggio matematico, la definizione topologica di limite corrisponde a: $\red{\forall U(\ell) \exists U(x_0): x\in U(x_0) \Rightarrow f(x) \in U(\ell)}$

> **La definizione successionale di limite e quella topologica sono equivalenti per $f: I \subseteq\mathbb{R} \to \mathbb{R}$ e $x_0\in\overline\mathbb{R}$ un punto di accumulazione per $I$ e $\ell \in \overline \mathbb{R}$.**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
$f: \mathbb{N} \to \mathbb{R}$ è incluso nella definizione topologica di limite con $I = \mathbb{N}$, $x_0 = +\infty$ e $\lim_{n\to\infty}f(n) = \ell \in\overline \mathbb{R}$.


## 2.4 Definizioni metriche di limite

Specificando nella definizione topologica di limite la forma esplicita degli intorni $U(\ell)$  e $U(x_0)$ nei casi $x_0 \in \mathbb{R} \cup \{+\infty\} \cup \{-\infty\}$ e $\ell \in \mathbb{R} \cup \{+\infty\} \cup \{-\infty\}$ si trovano le 9 definizioni metriche di limite, che non riportiamo.

# 3. Asintoti orizzontali, obliqui e verticali, limite per eccesso e per difetto e limite da destra e da sinistra

## 3.1 Asintoto orizzontale


>Definizione: Asintoto orizzontale
**Diremo che $f$ ha asintoto orizzontale $y = \ell \in \mathbb{R}$ per $x \to \pm\infty$ se $\lim_{x\to\pm\infty}f (x)= \ell$**

![image.png](13%20Limiti%20di%20funzioni/image.png)

## 3.2 Limite per eccesso e per difetto

>Definizione: Limite per eccesso e per difetto
>**Se $\ell \in \mathbb{R}, x_0 \in \overline \mathbb{R}$ si dice che $\lim_{x\to x_0}f(x)= \ell^+$ se $\lim_{x\to x_0} f(x)= \ell$ ed $\exists U(x_0): f(x) \ge \ell \ \forall x \in U(x_0), x\neq x_0.$ Si parla in questo caso di limite per eccesso.** 
>$$\forall \epsilon > 0 \exists \delta  > 0: 0<|x-x_0| < \delta \Rightarrow \ell\le f(x) < \ell + \epsilon$$
>
>**Se $\ell \in \mathbb{R}, x_0 \in \overline \mathbb{R}$ si dice che $\lim_{x\to x_0}f(x)= \ell^-$ se $\lim_{x\to x_0} f(x)= \ell$ ed $\exists U(x_0): f(x) \le \ell \ \forall x \in U(x_0), x\neq x_0.$ Si parla in questo caso di limite per difetto.** 
>$$\forall \epsilon > 0 \exists \delta  > 0: 0<|x-x_0| < \delta \Rightarrow \ell - \epsilon < f(x) \le \ell$$


## 3.3 Asintoto obliquo

>Definizione: Asintoto obliquo
**Diremo che $f$ ha asintoto obliquo $y = mx +q$, con $m \in \mathbb{R} \setminus\{0\}$ e $q \in \mathbb{R}$,  per $x \to \pm\infty$ se $\lim_{x\to\pm\infty}|f (x)- (mx +q)|= 0$**


Si noti che la quantità $|f (x)- (mx +q)|$ corrisponde alla distanza tra i due grafici al punto x misurata in verticale.

Si dimostra che $f (x)- (mx +q) = o(1),$ ossia che per $x\to \infty$ ${f (x)- (mx +q) \over 1} \to 0$. Si può quindi scrivere che $f (x) =  (mx +q) + o(1)$

![image.png](13%20Limiti%20di%20funzioni/image%201.png)

> Teorema
> **$f$  ha asintoto obliquo a $\pm \infty$ se $\lim_{x-\to\pm\infty} {f(x) \over x} = m \in \mathbb{R} \setminus\{0\}$ e $\lim_{x\to\pm\infty}f (x)- mx= q \in \mathbb{R}$. L’asintoto sarà quindi $y = mx +q$.**
> 

## 3.4 Limite da destra e da sinistra ed esistenza del limite

Talvolta è necessario distinguere il comportamento al limite di $f$ a seconda che $x$ si avvicini a $x_0$ da destra (per eccesso) o da sinistra (per difetto).

>Definizone: limite desto e sinitro
>**Data $f: I \subseteq \mathbb{R} \to \mathbb{R}$, $x_0 \in \mathbb{R}$ punto di accumulazione per $I$, diremo che $\lim_{x\to x_0^+}f (x)= + \infty$  se $\forall M > 0\exists \delta > 0: x_0 < x< x_0 + \delta \Rightarrow f(x) > M$.**
>
> **Data $f: I \subseteq \mathbb{R} \to \mathbb{R}$, $x_0 \in \mathbb{R}$ punto di accumulazione per $I$, diremo che $\lim_{x\to x_0^-}f (x)= + \infty$  se $\forall M > 0\exists \delta > 0: x_0 - \delta < x< x_0\Rightarrow f(x) > M$.**

>Teorema
> **Siano $f: I \subseteq \mathbb{R} \to \mathbb{R}$, $x_0 \in \mathbb{R}$ punto di accumulazione per $I$, $\ell \in \overline \mathbb{R}$. Allora vale che  $\lim_{x\to x_0}f (x)= \ell \Leftrightarrow \lim_{x\to x_0^+}f (x)= \ell = \lim_{x\to x_0^-}f (x)= \ell$.**
> 

Dalla proposizione appena scritta possiamo ricavare che se il limite destro e il limite sinistro di $f$ per $x\to x_0$ oppure non esiste uno dei due limiti, allora $\nexists\lim_{x\to x_0}f (x)$.

Se invece il dominio della funzione è definito su un intervallo chiuso $(a,b)$, ha senso unicamente chiedersi quale sia il limite da destra per $x$ che si avvicina ad $a$, mentre ha unicamente senso chiedersi quale sia quello da sinistra per $x$ che si avvicina a $b$.e

## 3.5 Asintoto verticale

>Definizione: Asintoto verticale
**Diremo che $f$ ha asintoto verticale $x= x_0 \in R$  se per $x\to x_0$ si ha $\lim_{x\to x_0^+}f (x)= \pm\infty$  oppure $\lim_{x\to x_0^-}f (x)= \pm \infty$ .**

![image.png](13%20Limiti%20di%20funzioni/image%202.png)

# 4. Limite finito al finito e continuità

Si noti che nella definizione di $\lim_{x\to x_0}f (x)= \ell$, con $x_0$  e $\ell$  finiti non importa che $f$ sia definita in $x_0$. Se è definita, allora non importa quale sia il valore assunto dalla funzione in quel punto.

>Definizone: continuità 
**Data $f: I \subseteq \mathbb{R} \to \mathbb{R}$, $x_0 \in \mathbb{R}$ punto di accumulazione per $I$, $x_0 \in I$, se $\lim_{x\to x_0}f (x)= f(x_0)$, diremo che $f$ è continua in $x_0$. Diremo che $f$ è continua in $I$ se $f$ è continua in $x_0$, $\forall x_0 \in I$. Scriveremo allora che $f\in C^0(I)$.**

Se una funzione è continua, allora possiamo riscrivere la definizione di limite finito al finito come $\forall \epsilon > 0 \exists \delta >0: |x-x_0|<\delta \Rightarrow |f(x) - f(x_0)| < \epsilon$. In aggiunta, utilizzando le definizione successionale di limite possiamo dedurre che $\forall x_n: x_n \in I \ \forall n \in \mathbb{N} , \lim_{n\to\infty}x_n = x_0$ allora $\lim_{n\to\infty} f(x_n) = f(x_0) = f(\lim_{n\to\infty}x_n)$, ossia **per le funzioni continue il limite scala all’argomento**.

# 5. Punti di discontinuità

Domandarsi se $f: (-\infty; 0)\cup(0; +\infty)\to \mathbb{R}$ definita da $f(x) = \frac{1}{x}$ sia continua o meno non ha senso secondo la definizione di continuità appena data, non essendo $f$ definita in $0$.

---

Siano d’ora in avanti **$f: I \subseteq \mathbb{R} \to \mathbb{R}$, $x_0 \in \mathbb{R}$ punto di accumulazione per $I$, $x_0 \in I$.**

## 5.1 Discontinuità eliminabile


>Definizione: Discontinuità eliminabile 
**Se $\exists \lim_{x\to x_0} f(x) = \ell\in \mathbb{R}$, con $\ell \ne f(x_0)$ diremo che $x_0$ è punto di discontinuità eliminabile per $f$.**

Questo significa che è possibile ridefinire $f$ in $x=x_0$ ponendo $\tilde{f}= \begin{cases} f(x),& x\ne x_0\\ \ell, & \ x = x_0\end{cases}$
La funzione così definita sarà continua in  $x_0$.

Similmente se $f$ non è definita in $x_0$ ma esiste il limite della funzione per $x\to x_0$, si può estendere $f$ per continuità in $x_0$. La funzione così così costruita ha dominio più grande di $f$, coincide con $f$ sul dominio di quest’ultima ed è continua in $x_0$

![image.png](13%20Limiti%20di%20funzioni/image%203.png)

## 5.2 Discontinuità di I specie

>Definizione: Discontinuità di I specie
**Se $\exists \lim_{x\to x_0^-} f(x) =\ell_1, \exists \lim_{x\to x_0^+} f(x)= \ell_2, \ell_1\ne\ell_2$, diremo che $x_0$ è punto di discontinuità di I specie o di tipo salto per $f$, con salto $s(x_0) = \ell_2-\ell_1$**


Se $f(x_0) = \lim_{x\to x_0^-} f(x)$ diremo che $f$ è continua da sinistra, altrimenti se 
$f(x_0) = \lim_{x\to x_0^+} f(x)$ diremo che $f$ è continua da destra.

![image.png](13%20Limiti%20di%20funzioni/image%204.png)

## 5.3 Discontinuità di II specie

>Definizione: Discontinuità di II specie
>**Se $\exists \lim_{x\to x_0^-} f(x) =\ell_1, \exists \lim_{x\to x_0^+} f(x)= \ell_2$ con almeno uno dei due infinito oppure non esistente, diremo che $x_0$ è punto di discontinuità di II specie per $f$.**


![image.png](13%20Limiti%20di%20funzioni/image%205.png)