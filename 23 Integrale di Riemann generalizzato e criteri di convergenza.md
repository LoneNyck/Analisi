# 23. Integrale di Riemann generalizzato e criteri di convergenza per integrali impropri

Tags: Integrali
Data lezione: 04/12/2024

# 1. Integrale di Riemann generalizzato

Vogliamo definire l’integrale anche per funzioni da $I\to \R$, con $I \subseteq\R$ intervallo che possa essere non chiuso o non limitato o dove $f$  possa essere illimitata in $I$ .

>Definizione
> **Sia $f:[a,b)\to \R$ con $a\in \R$  e $b\in\R\cup \{+\infty\}$, $f$  possibilmente illimitata per $x\to b^-$. Sia $f$  Riemann integrabile in $[a,h], \forall h \in (a,b)$. Definiamo**
>
>$$
>\int_a^bf(x)\ dx = \lim_{h\to b^-}\int_a^hf(x)\ dx 
>$$
> **se tale limite esiste in $\overline \R$.**

Inoltre se tale limite esiste finito, $f$ si dice **Riemann integrabile in senso improprio** o generalizzato e $\int_a^bf(x)\ dx$ converge.
Se tale limite esiste infinito, $f$ non è Riemann integrabile nè Riemann integrabile in senso improprio e $\int_a^bf(x)\ dx$ diverge.
Se tale limite non esiste, $f$ non è Riemann integrabile né Riemann integrabile in senso improprio e $\int_a^bf(x)\ dx$ non esiste.


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**

Se $f:[a,b)\to \R$ è Riemann integrabile in $[a,h], \forall h \in (a,b)$ e se $f$  ammette primitiva $F:[a,b)\to \R$, allora $\int_a^h f(x)\ dx= F(h)-F(a)$ per il teorema fondamentale del calcolo integrale I.

$$
\int_a^bf(x)\ dx = \lim_{k\to a^+}\int_k^bf(x)\ dx = \lim_{k\to a^+}F(b)-F(k)= [F(x)]_{a^+}^{b}
$$
se tale limite esiste in $\overline \R$.

>Definizione:
>**Sia $f:(a,b]\to \R$ con $a\in \R \cup \{-\infty\}$ e $b\in\R$, $f$  possibilmente illimitata per $x\to a^+$. Sia $f$  Riemann integrabile in $[k,b], \forall k \in (a,b)$. Definiamo**
>
>$$
>\int_a^bf(x)\ dx = \lim_{k\to a^+}\int_k^bf(x)\ dx 
>$$
>**se tale limite esiste in $\overline \R$.**

Inoltre se tale limite esiste finito, $f$ si dice **Riemann integrabile in senso improprio** o generalizzato e $\int_a^bf(x)\ dx$ converge.
Se tale limite esiste infinito, $f$ non è Riemann integrabile né Riemann integrabile in senso improprio e $\int_a^bf(x)\ dx$ diverge.
Se tale limite non esiste, $f$ non è Riemann integrabile né Riemann integrabile in senso improprio e $\int_a^bf(x)\ dx$ non esiste.


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**

Se $f:(a,b]\to \R$ è Riemann integrabile in $[k,b], \forall k \in (a,b)$ e se $f$  ammette primitiva $F:(a,b]\to \R$, allora $\int_k^b f(x)\ dx= F(b)-F(k)$ per il teorema fondamentale del calcolo integrale I.

$$
\int_a^bf(x)\ dx = \lim_{k\to a^+}\int_k^bf(x)\ dx = \lim_{k\to a^+}F(b)-F(k)= [F(x)]_{a^+}^{b}
$$

se tale limite esiste in $\overline \R$.


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
A volte, per distinguere l’integrale di Riemann in $[a,b]$ che abbiamo visto in precedenza da quello improprio9, si parla nel primo caso di integrale di Riemann in $[a,b]$ in senso proprio.


In particolare si può dimostrare svolgendo tutti i calcoli che 

Grazie all’integrale di Riemann in senso improprio è possibile calcolare il carattere di integrali come $\int_0^1\frac 1{x^\alpha} \ dx$ e $\int_1^\infty\frac 1{x^\alpha} \ dx$.

$$
\int_0^1\frac 1{x^\alpha} \ dx \,\,\,\,\,\begin{cases}\text{converge}, &\alpha \le 1\\\text{diverge},& \alpha > 1  \end{cases}
$$

$$
\int_1^\infty\frac 1{x^\alpha} \ dx \,\,\,\,\,\begin{cases}\text{diverge}, &\alpha \le 1\\\text{converge},& \alpha > 1  \end{cases}
$$

>Definizione
>**Sia $f:(a,b)\to \R$ con $a<b, a,b \in \overline \R$, $f$  possibilmente illimitata per $x\to a^+$ o per $x \to b^-$. Sia $f$  Riemann integrabile in $[k,h], \forall k,h \in (a,b), k<h$. Definiamo** 
>
>$$
>\int_a^bf(x)\ dx = \lim_{k\to a^+, h \to b^-}\int_k^h f(x)\ dx 
>$$
>**se tale doppio limite esiste in $\overline \R$.**

Inoltre se tale doppio limite esiste finito, $f$ si dice **Riemann integrabile in senso improprio** o generalizzato e $\int_a^bf(x)\ dx$ converge.
Se tale doppio limite esiste infinito, $f$ non è Riemann integrabile né Riemann integrabile in senso improprio e $\int_a^bf(x)\ dx$ diverge.
Se tale doppio limite non esiste, $f$ non è Riemann integrabile né Riemann integrabile in senso improprio e $\int_a^bf(x)\ dx$ non esiste.


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Equivale a chiedere che comunque sia fissata $c \in (a,b)$ $f$ sia Riemann integrabile in senso improprio in $(a,c]$ e in $[c,b)$. I due limiti vengono presi indipendentemente e

$$
\int_a^bf(x)\ dx = \int_a^cf(x)\ dx+\int_c^bf(x)\ dx
$$

$$
\lim_{k\to a^+, h \to b^-}\int_k^h f(x)\ dx = \lim_{k\to a^+}\int_k^bf(x)\ dx + \lim_{h\to b^-}\int_a^hf(x)\ dx
$$


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**

Se almeno uno tra i due limiti appena scritti non esiste oppure se esistessero entrambi infiniti ma di segno discorde, allora $\int_a^bf(x)\ dx$ non esiste. 

Nel caso in cui esistano entrambi finiti o infiniti di segno concorde, oppure uno finito e l’altro infinito, allora esisterebbe $\int_a^bf(x)\ dx$.


# 2. Criteri di convergenza per integrali generalizzati

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Se $f:[a,b)\to \R$ è Riemann integrabile in $[a,h], \forall h \in (a,b)$ e $f(x)\ge 0$, allora $\int_a^hf(x)\ dx$  è una funzione di $h$  crescente, quindi per il teorema di esistenza del limite per funzioni monotone in intervallo ammette limite in $\overline \R$  per $h\to b^-$.


## 2.1 Criterio del confronto
>Teorema: Criterio del confronto inetegrale
> **Siano $f,g:[a,b]\to\R$ tali che $f,g$  siano Riemann integrabili in $[a,h],\forall h \in (a,b)$. Supponiamo $\exists x_0\in (a,b):0\le f(x)\le g(x) , \forall x \in [x_0,b).$
Allora $\int_a^b f(x) \ dx , \int_a^b g(x) \ dx$  esistono in $\overline \R$ e inoltre vale che:**
> 
> 1. **Se $\int_a^b f(x) \ dx$  diverge, allora anche $\int_a^b g(x) \ dx$   diverge;**
> 2. **Se $\int_a^b g(x) \ dx$   converge, allora anche $\int_a^b f(x) \ dx$   converge.**
> 
> **Inoltre vale che $\int_{x_0}^b f(x) \ dx   \le \int_{x_0}^b g(x) \ dx$  .**
> 

## 2.2 Criterio del confronto asintotico
>Teorema: Criterio del confronto asintotico
> **Siano $f,g:[a,b]\to\R$ tali che $f,g$  siano Riemann integrabili in $[a,h],\forall h \in (a,b)$. Supponiamo $\exists x_0\in (a,b): f(x)\ge 0,  g(x) \ge 0, \forall x \in [x_0,b).$
Allora, se $f\sim g$ per $x\to b^-$, $\int_a^b f(x) \ dx , \int_a^b g(x) \ dx$  esistono entrambi in $\overline \R$ e i due integrali hanno lo stesso carattere, ossia o convergono entrambi, o divergono a $+\infty$**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**

- $\int_0^1 \frac 1 {x^\alpha} \ dx$ **converge per $\alpha < 1$  e diverge per $\alpha \ge 1$.**
- **$\int_1^\infty \frac 1 {x^\alpha} \ dx$ converge per $\alpha > 1$  e diverge per $\alpha \le 1$.**

## 2.3 Convergenza assoluta

>Definizione: Convergenza assoluta
**Sia $f:I\subseteq \R \to \R, I$  intervallo. Diremo che $f$ è assolutamente integrabile in senso improprio secondo Riemann in $I$  se $|f|$ è integrabile in senso improprio secondo Riemann.**

>Teorema
> **Sia $f:I\to \R, I$  intervallo, integrabile in senso proprio secondo Riemann in $[h,k]\sub I, \forall h,k \in I$. Se $f$ è assolutamente integrabile in senso improprio secondo Riemann, allora essa è anche integrabile semplicemente in senso improprio secondo Riemann.
Inoltre, per monotonia dell’integrale, vale $|\int_a^b f(x) \ dx|\le \int_a^b |f(x)| \ dx$.**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**

- $f$ integrabile in senso **proprio** $\Rightarrow$  $|f|$  integrabile in senso **proprio**. Il viceversa è falso.
- $|f|$ integrabile in senso **improprio** $\Rightarrow$  $f$  integrabile in senso **improprio**. Il viceversa è falso.

## 2.4 Criterio del confronto integrale per serie

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
C’è un collegamento tra serie ed integrali impropri.

$$
\sum_{n=1}^\infty a_n \leftrightarrow \int_1^\infty g(x) \ dx \\
\text {con }g(x) = a_n , \forall x \in [n,n+1], \forall n \in \mathbb{N}, n\ge 1
$$

Si può dimostrare che $\sum a_n$ converge, diverge o è irregolare se e solo se $\int g(x) \ dx$ rispettivamente converge, diverge o è irregolare.

>Teorema
> **Siano $M \in \mathbb{N}$ , $f:[M,\infty)\to\R$ decrescente e non negativa. Allora 
$\sum_{n=1}^\infty f(n)$ converge o diverge se e solo se $\int_{1}^\infty f(x) \ dx$ converge o diverge rispettivamente.**
> 
> 
> **Inoltre $\int_{M}^\infty f(x) \ dx\le \sum_{M}^\infty f(n) \le f(M)+\int_{M}^\infty f(x) \ dx$** 
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazioni**

Nelle ipotesi del teorema $\sum a_n$ è serie a termini positivi, quindi o converge o diverge per il teorema della convergenza o divergenza per serie a termini positivi [[11. Serie a termini definitivamente “positivi”](11%20Serie%20a%20termini%20definitivamente%20%E2%80%9Cpositivi%E2%80%9D%2012134a78851580ecafbef6bb3636d4ff.md), par. 2].

Il fatto che $f$ sia monotona e positiva implica che $\int_{1}^\infty f(x) \ dx$ è ben definito e o converge o diverge.
