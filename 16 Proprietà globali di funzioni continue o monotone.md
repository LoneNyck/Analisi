# 16. Proprietà globali di funzioni continue o monotone su un intervallo

Tags: Dimostrazione importante, Funzioni, Limiti
Data lezione: 06/11/2024

# 1. Teorema degli zeri
>Teorema degli zeri 
> **Sia $f: [a,b]\to \R$, $a,b \in \R, a < b,$ $f$ continua nel dominio e tale che $f(a) f(b) <0$. Allora $\exists x_0 \in [a,b]$ tale che $f(x_0) = 0$. Inoltre se $f$ è strettamente monotona, allora tale $x_0$ è unico.**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazioni**
- Il teorema dà condizioni che garantiscono che $f(x_0) = 0$ abbia soluzione.
- Esso garantisce inoltre che la soluzione $x_0$  sia in $(a,b)$.

## 1.1 Dimostrazione

- Chiamiamo $a_0 = a , b_0 = b$  e sia $c_0 = \frac{a_0+b_0}2$ il punto medio del segmento $a_0b_0$.
    - Se $f(c_0) = 0 \Rightarrow x_0= c_0$
    - Se $f(c_0)\ne 0$ vale che $f(c_0)f(a_0)<0$ oppure che $f(c_0)f(b_0)<0$, ma non entrambe contemporaneamente. 
    Mettiamoci nel primo caso e poniamo quindi $a_1 = a_0, b_1= c_0$ e sia $c_1= \frac{a_1+b_1}2$ il punto medio del segmento $a_1b_1$. 
    Si ripete quindi a questo punto l’algoritmo.
    Supponiamo ora che sia $f(c_1)f(b_1)<0$. Poniamo quindi $a_2 = c_1, b_2=b_1$ e sia $c_2 =\frac{a_2+b_2}2$ il punto medio del segmento $a_2b_2$. Si ripete quindi a questo punto l’algoritmo.
    
    L’algoritmo si conclude se si trova un $c_k$ tale che $f(c_k) = 0$. 
    
    Se ciò non accade, esso procede all’infinito: abbiamo così costruito due successioni $a_n$  e $b_n$ tali che:
    
    1. $a_n$  sia crescente e $b_n$  sia decrescente
    2. $f(a_n)f(b_n)<0$
    3. $0\le b_n-a_n= \frac{b-a}{2^n}$
    4. $a_n,b_n\in (a,b)$
    
    $a_n$  e $b_n$ sono due successioni monotone limitate per le proprietà i. e iv. quindi per il teorema dell’esistenza del limite per successioni monotone $\exists \lim _{n\to\infty}a_n = \overline a$ ed 
    $\exists \lim _{n\to\infty}b_n = \overline b$. Dal punto iii. deduciamo che 
    $\exists \lim _{n\to\infty}b_n -a_n = \overline b -\overline a = \lim_{n\to\infty}\frac{b-a}{2^n}=0$, quindi che $\overline b =\overline a$.
    Chiamiamo quindi $x_0 =\overline b =\overline a\in (a,b)$. Per continuità di $f$ possiamo dedurre che $\lim _{n\to\infty}f(a_n)=f(\lim _{n\to\infty}a_n) = f(x_0)$ e la stessa cosa può essere fatta per $b_n$.
    Per algebra dei limiti $\lim _{n\to\infty}f(a_n)f(b_n)=f^2(x_0)$.
    Per permanenza del segno, essendo da ii. $f(a_n)f(b_n)<0$, abbiamo che $\lim _{n\to\infty}f(a_n)f(b_n)=f^2(x_0)\le 0$, che può verificarsi solo nel caso in cui $f(x_0)= 0$.
    
- Passiamo ora a quanto riguarda la monotonia e l’unicità dell’eventuale zero.
    
    Se $f$ è strettamente crescente $f(x)> f(x_0), \forall x\in (x_0,b)$ e $f(x)< f(x_0), \forall x\in (a,x_0)$, mentre se $f$ è strettamente decrescente si ha che $f(x)< f(x_0), \forall x\in (x_0,b)$ e $f(x)> f(x_0), \forall x\in (a,x_0)$ e in ogni caso $f(x) \ne 0=f(x_0)$, per $x\ne x_0$
    

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" />**Osservazioni**

- Il teorema fornisce un algoritmo che produce approssimazioni della soluzione di $x_0$, in quanto $a_k$ cresce, $b_k$ decresce e $\lim_{n\to\infty}a_k=\lim_{n\to\infty}b_k= x_0$
- $\forall k \in \mathbb{N}$ vale che $0 \le x_0 -a_k \le b_k -a_k \le \frac{b-a}{2}$ e  $0 \le b_k - x_0 \le b_k -a_k \le \frac{b-a}{2}$

# 2. Teorema di Weierstrass

>Definizone: minimo e massimo
>**Se $f: I \subseteq \R \to \R$ e $x_m\in I :  f(x_m) =\min f(x)$ per $x\in[a,b]$, $x_m$ si dice punto di minimo per $f$ e $f(x_m)$ si dice minimo della funzione.**
>**Se $f: I \subseteq \R \to \R$ e $x_M\in I :  f(x_M) =\max f(x)$ per $x\in[a,b]$, $x_M$ si dice punto di massimo per $f$ e $f(x_M)$ si dice massimo della funzione.**

>Teorema di Weierstrass
> **Sia $f: [a,b]\to \R$, $a,b \in \R, a < b,$ $f$ continua nel dominio. Allora $f$ ammette massimi e minimi assoluti in $[a,b]$, ossia $\exists x_m, x_M\in [a,b]: f(x_m) \le f(x)\le f(x_M) \forall x\in [a,b]$.
Inoltre $f(x_m) = \min f(x), x\in [a,b]$ e $f(x_M) = \max f(x), x\in [a,b]$.**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" />**Osservazioni**

- Se $f:[a,b] \to \R$ è continua, per il teorema di Weierstrass essa è limitata in  $[a,b]$ in quanto $\sup f = \max f$ e $\inf f = \min f$
- Se $f$ non è continua o se $I$  non è chiuso o non è limitato, allora il teorema di Weierstrass è falso.

# 3. Teorema dei valori intermedi

>Teorema dei valori intermedi
> **Sia $f:[a,b] \to \R$ continua. Allora $\forall \lambda \in \R$ compreso tra $m= \min f$ e $M = \max f$ (inclusi), esiste $x_0\in [a,b]: f(x_0 ) = \lambda$.**
> 

## 3.1 Dimostrazione

Per il teorema di Weierstrass $f$ ammette massimo e minimo assoluti in $[a,b]$, quindi $\exists x_m, x_M:f(x_m)=\min f(x)=m$ e $f(x_M)=\max f(x) = M$. 

Se $\lambda = m$  oppure $\lambda = M$ abbiamo concluso, avendo trovato i valori per i quali questo si verifica.

Se $\lambda \in (m,M)$, assumiamo $x_m<x_M$  per comodità. Consideriamo la funzione 
$g:[x_m,x_M]\to \R$, $g(x) = f(x)-\lambda$. Possiamo dedurre che $g$ sia continua dal fatto che $[x_m,x_M]\subseteq [a,b]$ e dal fatto che $f$ sia continua. Avendo $m<\lambda< M$ - il caso uguale è già stato preso in considerazione - possiamo concludere che
$g(x_m)= f(x_m)-\lambda=m-\lambda<0$
$g(x_M) = f(x_M)-\lambda = M-\lambda >0$
Per il teorema degli zeri $\exists x_0\in (x_m,x_M)\subseteq(a,b)$ tale che $g(x_0) = 0$. Questo equivale a dire che $f(x_0)= \lambda$.

## 3.2 Conseguenza del teorema dei valori intermedi
>Corollario
> **Se $f:[a,b] \to \R$ è continua, allora $\operatorname{Im} f= [m,M]$ con $m = \min f$ e $M = \max f$.**
> 

>Corollario
> **Se $f:I \subseteq \R \to \R$ è continua in $I$, con $I$  intervallo, allora $\operatorname{Im} f$ è un intervallo.**
> 

# 4. Teorema sul limite di funzioni monotone

Segue un teorema per funzioni monotone: esse è stato diviso nei casi in cui la funzione sia crescente o decrescente.
>Teorema
> **Sia $f:(a,b) \to \R$  una funzione monotona crescente. Allora $\forall x_0\in (a,b)$ esistono finiti $\lim_{x\to {x_0}^-}f(x)$ e $\lim_{x\to {x_0}^+}f(x)$ $\in \R$.
Inoltre $\lim_{x\to {x_0}^-}f(x) = \sup f(x) , x \in (a,x_0)$ e $\lim_{x\to {x_0}^+}f(x)= \inf f(x), x \in (x_0,b)$.
Ne consegue che $\lim_{x\to {x_0}^-}f(x)\le f(x_0) \le\lim_{x\to {x_0}^+}f(x)$**
> 

Inoltre esistono, eventualmente infiniti $\lim_{x\to {a}^+}f(x)= \inf f(x) , x \in (a,b)$ e $\lim_{x\to {b}^-}f(x)= \sup f(x), x \in (a,b)$.
>Teorema
> **Sia $f:(a,b) \to \R$  una funzione monotona decrescente. Allora $\forall x_0\in (a,b)$ esistono finiti $\lim_{x\to {x_0}^-}f(x)$ e $\lim_{x\to {x_0}^+}f(x)$ $\in \R$.
Inoltre $\lim_{x\to {x_0}^-}f(x) = \inf f(x) , x \in (a,x_o)$ e $\lim_{x\to {x_0}^+}f(x)= \sup f(x), x \in (x_0,b)$.
Ne consegue che $\lim_{x\to {x_0}^-}f(x)\ge f(x_0) \ge\lim_{x\to {x_0}^+}f(x)$**
> 

Inoltre esistono, eventualmente infiniti $\lim_{x\to {a}^+}f(x)= \sup f(x) , x \in (a,b)$ e $\lim_{x\to {b}^-}f(x)= \inf f(x), x \in (a,b)$.


>Corollario
> **Se $f: (a,b)\to \R$ è monotona, i suoi eventuali punti di discontinuità in $(a,b)$  sono di tipo salto. Inoltre in $x= a$  e in $x = b$, $f$  ammette limite finito - ed è quindi ivi prolungabile per continuità - oppure infinito - ed è quindi ivi presenta un asintoto verticale.**
> 

# 5. Continuità e invertibilità

Abbiamo già visto in [6. Nozioni elementari sulle funzioni](6%20Nozioni%20elementari%20sulle%20funzioni%2011034a78851580bf8b22e74f29991a40.md), 8.1,  che la monotonia stretta implica l’invertibilità e che la funzione inversa così ottenuta sarà anch’essa monotona. Il viceversa in generale però non è vero, ossia una funzione invertibile non è strettamente monotona. Se $f$ è continua questo però non è vero.
>Teorema
> **Sia $f:I \subseteq \R \to \R$, con $I$  intervallo e $f$  continua. $f$ invertibile $\Leftrightarrow$  $f$ strettamente monotona.**
> 

In tal caso inoltre $f^{-1}: \operatorname{Im} f \subseteq \R \to \R$ è strettamente monotona come $f$, $f^{-1}$ ha come dominio un intervallo e $f^{-1}$ è continua nel suo dominio.

Una funzione continua e invertibile ha inversa continua. In particolare sono continue nei loro domini: 

- $x^{1/n}, \forall n \in \mathbb{N}$
- $\arcsin x , \arccos x , \arctan x$

- $\log_a x, a > 0, a \ne 1$
- $\sinh^{-1} x , \cosh^{-1} x$