# 14. Teoremi sui limiti di funzioni

Tags: Funzioni, Limiti
Data lezione: 30/10/2024

>Definizione: Definitivamente
**Siano $f: I \subseteq {\mathbb{R}} \to {\mathbb{R}}$, $x_0 \in {\mathbb{R}}$ punto di accumulazione per $I$. Diremo che una funzione $f$ soddisfa una proprietà $p$ definitivamente per $x\to x_0$se $\exists U(x_0)$ intorno di $x_0$ tale che $p$ sia soddisfatta $\forall x \in U(x_0), x\ne x_0$.** 

# 1. Teorema del confronto
>Teorema del condronto
> **Siano $f,g,h: I \subseteq {\mathbb{R}} \to {\mathbb{R}}$, $x_0 \in \overline{\mathbb{R}}$ punto di accumulazione per $I$. Se $\exists\lim_{x\to x_0}f(x)=\lim_{x\to x_0}h(x)=\ell$ e vale definitivamente che $f(x) \le g(x) \le h(x)$ allora $\exists\lim_{x\to x_0}g(x)= \ell$**
> 

## 1.1 Teorema del confronto per funzioni con limite infinito.
>Teorema 
> **Siano $f,g: I \subseteq {\mathbb{R}} \to {\mathbb{R}}$, $x_0 \in \overline{\mathbb{R}}$ punto di accumulazione per $I$. Supponiamo sia $f(x) \le g(x)$  definitivamente per $x\to x_0$.**
> 
> 1. $\exists\lim_{x\to x_0}f(x)= +\infty$ $\Rightarrow$ $\exists\lim_{x\to x_0}g(x)= +\infty$
> 2. $\exists\lim_{x\to x_0}g(x)= -\infty$ $\Rightarrow$ $\exists\lim_{x\to x_0}f(x)= -\infty$

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
I teoremi del confronto valgono anche per limiti da destra e da sinistra separatamente.


## 1.2 Corollario del teorema del confronto

1. **Date due funzioni $f$ e $g$ : $|f| \le |g |$ definitivamente per $x\to x_0$ ed 
$\exists\lim_{x\to x_0}g=0$ $\Rightarrow$ $\exists\lim_{x\to x_0}f=0$**
2. **Date due funzioni $f$ e $g$  tali che $f$ sia limitata ed $\exists\lim_{x\to x_0}g=0$ $\Rightarrow$ $\exists\lim_{x \to x_0}f(x)g(x)=0$**

# 2. Teorema della permanenza del segno

## 2.1 Prima forma

>Teorema
> **Data una funzione $f$, se $\exists\lim_{x\to x_0}f(x)=\ell$ e $\ell>0$
$\Rightarrow$  $f(x) > 0$ definitivamente per $x\to x_0$. 
Similmente se $\ell<0$
$\Rightarrow$ $f(x) < 0$ definitivamente per $x\to x_0$.**
> 

### 2.1.1 Dimostrazione

Assumiamo $x_0$  e $\ell \in {\mathbb{R}}$. 
Per la definizione di limite abbiamo che 
$\forall \epsilon >0 \exists \delta > 0:0<|x-x_0|<\delta \Rightarrow \ell-\epsilon < f(x)<\ell+\epsilon$.

Adottando $\epsilon = \frac\ell 2$ abbiamo che $\ell -\epsilon = \frac \ell 2 >0$, che implica che $f(x) >0$ definitivamente.

## 2.2 Seconda forma
>Teorema
> **Data una funzione $f$, se $\exists\lim_{x\to x_0}f(x)=\ell$ e $f(x) \ge 0$
$\Rightarrow$  $\ell \ge 0$ definitivamente per $x\to x_0$. 
Similmente se $f(x) \le 0$
$\Rightarrow$ $\ell \le 0$ definitivamente per $x\to x_0$.**
> 

### 2.2.1 Dimostrazione

Utilizziamo per questa dimostrazione la definizione successionale di limite: sia $x_n$  una successione qualsiasi tale che $x_n \in D_f \ \forall n \in \mathbb{N}$, $x_n \neq x_0 \ \forall n \in \mathbb{N}$ e $\lim_{n\to\infty}x_n = x_0$; allora $\lim_{n\to\infty}f(x_n) = \ell$.

Poiché $f(x)\ge 0$ definitivamente per $x\to x_0$ e $\lim_{n\to\infty}x_n = x_0$, definitivamente in $n\in \mathbb{N}$ vale che $f(x_n) \ge 0.$ Per il teorema di permanenza del segno per successioni quindi $\ell \ge 0$.

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Anche se $f(x) > 0$, il limite sarebbe ancora $\ell \ge 0$: basta pensare ad una funzione come $1\over x^2$. Il maggiore stretto, in questo caso non passa al limite.


![image.png](14%20Teoremi%20sui%20limiti%20di%20funzioni/image.png)

# 3. Teorema sull’algebra dei limiti e aritmetizzazione parziale di infinito.

Siano $f$ e $g$ due funzioni ed $\exists\lim_{x\to x_0}f(x)=\ell_1$ ed $\exists\lim_{x\to x_0}g(x)=\ell_2$, con $\ell_1, \ell_2, x_0 \in \overline {\mathbb{R}}$.
Allora:

1. $\lim_{x\to x_0}f(x)\pm g(x) = \ell_1\pm\ell_2$
2. $\lim_{x\to x_0}f(x)g(x)= \ell_1\ell_2$
3. $\lim_{x\to x_0}{f(x)\over g(x)}= {\ell_1 \over \ell_2}$, con $g(x) \ne 0$ in un intorno di $x_0$, salvo al più $x_0$
4. $\lim_{x\to x_0}f(x)^{g(x)} = {\ell_1}^{\ell_2}$, con $f(x)^{g(x)}$ ben definita in un intorno di $x_0$, salvo al più $x_0$
5. $\lim_{x\to x_0}f(x)^\alpha = {\ell_1}^\alpha$, con $f(x)^{\alpha}$ ben definita in un intorno di $x_0$, salvo al più $x_0$

a meno di forme di indeterminazione $\infty - \infty, 0\cdot \infty, {0\over 0}, {\infty \over \infty}, 1^\infty, \infty^0, 0^0$ oppure del caso $c\over 0$, con $c\in \overline {\mathbb{R}}\setminus\{0\}$ e $0$ né $0^+$ né $0^-$.

# 4. Teorema sull’algebra delle funzioni continue.

Siano $f$ e $g$ sono funzioni continue in $x_0\in{\mathbb{R}}$, cioè $\lim_{x\to x_0}f(x)=f(x_0)$ e $\lim_{x\to x_0}g(x)=g(x_0)$.
Allora:

1. $\lim_{x\to x_0}f(x)\pm g(x) = f(x_0)\pm g(x_0)$
2. $\lim_{x\to x_0}f(x)g(x)= f(x_0)g(x_0)$
3. $\lim_{x\to x_0}{f(x)\over g(x)}= {f(x_0) \over g(x_0)}$, con $g(x) \ne 0$ in un intorno di $x_0$, salvo al più $x_0$
4. $\lim_{x\to x_0}f(x)^\alpha = {f(x_0)}^\alpha$, con $f(x)^{\alpha}$ ben definita in un intorno di $x_0$, salvo al più $x_0$

## 4.1 Teorema sulle funzioni elementari
>Teorema
> **Le funzioni elementari sono continue nel loro campo di esistenza.**
> 

Come conseguenza del teorema sono continue tutte le seguenti:

- potenze: $x^\alpha$
- esponenziali: $a^x$
- logaritmi: $\log_ax$
- modulo: $|x|$

- funzioni trigonometriche: $\sin x, \cos x, \tan x, \cot x$
- inverse delle funzioni trigonometriche: $\arcsin x, \arccos x, \arctan x$
- funzioni iperboliche: $\sinh x, \cosh x, \tanh x$

# 5. Teorema del cambio di variabile
>Teorema: cambio di variabile
> **Siano $f$ e $g$ due funzioni per cui sia definito la composizione 
$f \circ g= f(g(x))$ almeno in un intorno $U(x_0)$ di $x_0$ - salvo al più $x_0$. 
Se:**
> 
> 1. **$\lim_{x\to x_0}g(x) = t_0\in \overline {\mathbb{R}}$**
> 2. **$\lim_{t\to t_0}f(t)= \ell**$
> 3. **$g(x) \ne t_0$ definitivamente per $x \to x_0$**
> 
> **allora $\lim_{x\to x_0}f(g(x))= \lim_{t\to t_0}f(t)= \ell$**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
L’ipotesi iii. non è necessaria nel caso in cui $t_0 = \pm \infty$ e se $f$ è continua in $t_0$, ossia se $f(t_0) = \ell$.


## 5.1 Continuità della composizione di funzioni continue
>Teorema
> **Sia g definita in un intorno di $x_0$ e continua in $x_0$, cioè 
$\lim_{x\to x_0}g(x) = g(x_0)$. 
Sia f definita in un intorno di  $t_0=g(x_0)$ e continua in $t_0$, cioè $\lim_{t\to t_0}f(t) = f(t_0)$.
Allora $f\circ g$ è definita in un intorno di $x_0$ ed è continua in $x_0$, ossia $\lim_{x\to x_0}f(g(x)) = f(g(x))= f(g(x_0))$.**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
$\lim_{x\to x_0}f(g(x)) = f(g(x_0)= f(\lim_{x\to x_0}g(x))$ 

**Somme, differenze, prodotti e quozienti con denominatore non nullo, potenze ben definite e composizioni di funzioni continue sono tutte continue.**