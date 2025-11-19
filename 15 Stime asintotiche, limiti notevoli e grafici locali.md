# 15. Stime asintotiche, limiti notevoli e grafici locali per funzioni

Tags: Dimostrazione importante, Funzioni, Limiti
Data lezione: 31/10/2024

# 1. Asintotici ed o-piccoli

Segue la definizione di asintotico ed o-piccolo, già vista anche per le successioni in precedenza in [9. Confronti e stime asintotiche per successioni](9%20Confronti%20e%20stime%20asintotiche%20per%20successioni%2011a34a788515807b9271e31a474c27eb.md), par. 2.


>Definizione: o-piccolo e asintotico
>**Date due funzioni $f$  e $g$ e $x_0 \in \overline \mathbb{R}$ diremo che**
>- **${f(x)\sim g(x)}$ per $x\to x_0$ se $\lim_{x\to x_0}{f(x)\over g(x)} = 1$.**
>- **${f(x) = o(g(x))}$ per $x\to x_0$ se $\lim_{x\to x_0}{f(x)\over g(x)} = 0$.**

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**

- $\lim_{x\to x_0}{f(x)\over g(x)} = \lambda \in \mathbb{R} \setminus \{0\}$ $\Rightarrow$ $f(x) \sim \lambda g(x)$ , $x\to x_0$.
- $\lim_{x\to x_0}{f(x)\over g(x)} = \pm \infty$ $\Rightarrow$ $g(x) = o(f(x))$ , $x\to x_0$.

Inoltre è possibile stabilire una relazione tra $o$-*piccolo* e asintotico

$$
{f(x) \sim g(x) \Leftrightarrow f(x) = g(x) + o(g(x))\Leftrightarrow f(x) - g(x)= o(g(x)), x\to x_0}
$$

### 1.0 comma 1 - Dimostrazione

La dimostrazione è abbastanza semplice e si basa interamente sulle definizioni di asintotico ed o-piccolo insieme con algebra dei limiti. 
$f$ e $g$ sono asintotici tra loro se il limite del loro rapporto tende a $1$. Ora, spostando $1$ dentro al limite e facendo denominatore comune otteniamo che $\lim_{x\to x_0}{f(x)-g(x)\over g(x)} = 0$, ossia che $f(x) - g(x)= o(g(x)), x\to x_0$.

## 1.1 Proposizioni sugli asintotici

1. Se $f_1 \sim f_2$ e $g_1 \sim g_2$ per $x\to x_0$ allora:
    1. $f_1g_1\sim f_2g_2, x\to x_0$
    2. $\frac{f_1}{g_1}\sim \frac{f_2}{g_2} x\to x_0$
    3. $(f_1)^\alpha=(f_2)^\alpha, x\to x_0$

La relazione di asintotico può quindi essere usata senza limitazioni per quanto riguarda **prodotti**, **rapporti** e **potenze**.

1. Se $f\sim g$ per $x\to x_0$ allora $\exists \lim_{x\to x_0}f(x)\in \overline\mathbb{R}$ $\Leftrightarrow$ $\exists \lim_{x\to x_0}g(x)\in \overline \mathbb{R}$. Inoltre, se i due limiti esistono, essi sono uguali.

### 1.1 comma 1 - Dimostrazione

1. Tutte e tre le dimostrazioni consistono nello svolgere il rapporto tra il termine a sinistra e a destra dell’asintotico e utilizzare l’algebra dei limiti per verificare che quest’ultimo vada a $1$.
2. È possibile riscrivere $f(x) = \frac{f(x)}{g(x)}g(x)$. Esistendo il limite di $g(x)$ per $x\to x_0$ in $\overline \mathbb{R}$, per algebra dei limiti ed aritmetizzazione di infinito possiamo scrivere che $\lim_{x\to x_0}\frac{f(x)}{g(x)}g(x)= 1\cdot\ell = \ell$ essendo le due funzioni asintotiche per ipotesi.

---

In generale, date $f\sim f_1, g_1 \sim g_2 , x \to x_0$ senza ulteriori condizioni:

1. $f_1 \pm g_1 \nsim  f_2 \pm g_2$
2. $\log(f_1)  \nsim  \log(f_2)$
3. $e^{f_1} \nsim  e^{f_2}$

La relazione di asintotico **NON** vale quindi per la **somma**, per **l’esponenziale** e per il **logaritmo** a meno di ulteriori condizioni.

# 2. Limiti notevoli

Seguono una serie di limiti notevoli, con le rispettive relazioni di asintotico e gli o-piccoli

- $\lim_{x\to 0}{\sin x \over x} = 1$
    - $\sin x \sim x$
    - $\sin x = x +o(x)$
- $\lim_{x\to 0}{1 - \cos x\over x^2} = {1\over 2}$
    - $1-\cos x \sim {x^2\over 2}$
    - $\cos x =  1 - {x^2\over 2} + o({x^2\over 2})$
- $\lim_{x\to 0}{\tan x \over x} = 1$
    - $\tan x \sim x$
    - $\tan x = x + o (x)$

- $\lim_{x\to \pm \infty}(1+{ 1\over x})^x = e$
- $\lim_{x\to 0}{\log(1+x) \over x} = 1$
    - $\log(1+x) \sim x$
    - $\log(1+x) = x + o(x)$
- $\lim_{x\to 0}{e^x - 1 \over x} = 1$
    - $e^x -1 \sim x$
    - $e^x -1 = x + o (x)$
- $\lim_{x\to 0}{(1+x)^\alpha - 1 \over x} = \alpha$
    - $(1+x)^\alpha -1 \sim x$
    - $(1+x)^\alpha = 1+x+o(x)$

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Si noti che se $\epsilon(x)$ è una funzione tale per cui $\lim_{x\to x_0}\epsilon (x) = 0$, allora è possibile applicare il teorema di cambio variabile visto in [14. Teoremi sui limiti di funzioni](14%20Teoremi%20sui%20limiti%20di%20funzioni%2012f34a78851580fbbc8af41cb407c019.md), par. 5. 


# 3. Gerarchia degli infinti


Siano $a > 1, \alpha, \beta >0$.
 
- $\lim_{x\to \infty}{(\log_a x)^\alpha \over x^\beta} = 0$, che significa $(\log_a x)^\alpha = o(x^\beta)$, $x\to x_0$
- $\lim_{x\to \infty}{x^\beta \over a^x}= 0$, che significa $x^\beta = o(a^x)$, $x\to x_0$

Si noti che se $\lim_{x\to x_0}f(x) = \infty$, allora $\lim_{x\to x_0}{(\log_a f(x))^\alpha \over (f(x))^\beta} = 0$ e $\lim_{x\to x_0}{(f(x))^\beta \over a^{f(x)}}= 0$ per il teorema di cambio della variabile.

# 4. Grafici locali

Le stime tramite sviluppi asintotici servono per il calcolo dei limiti, ma anche per tenere traccia dei grafici qualitativi - probabili! -  di una funzione in un intorno di $x_o \in \overline \mathbb{R}$.  Si tenga a mente che per uno studio rigoroso e preciso è comunque necessario l’utilizzo di derivate. Si noti comunque che in generale non è vero che se $f\sim g$ per $x\to x_0$, allora vicino ad $x_0$  i grafici di $f$ e di $g$  si assomigliano.