# 19. Convessità e concavità

Tags: Derivate, Dimostrazione importante
Data lezione: 22/11/2024


>Definizone convessità
>**Una funzione $f:I \subseteq \mathbb{R}\to \mathbb{R}$, con $I$  intervallo, si dice convessa in $I$ se 
$\forall x_0,x_1\in I , \forall t \in [0,1]$ vale che $f(tx_1+(1-t)x_0)\le tf(x_1)+(1-t)f(x_0)$. Una funzione si dice strettamente convessa se $\forall x_0,x_1\in I , \forall t \in (0,1)$ vale che $f(tx_1+(1-t)x_0) < tf(x_1)+(1-t)f(x_0)$.**

>Definizione: concavità
>**Una funzione $f:I \subseteq \mathbb{R}\to \mathbb{R}$, con $I$  intervallo, si dice concava se $-f$ è convessa.**


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Dati due punti in $\mathbb{R}^2$ $\underline P_0(x_0,y_0), \underline P_1(x_1,y_1)$ , l’insieme dei punti 
$\underline P_t=(1-t)\underline P_0 + t\underline P_1 = \underline P_0 + t(\underline P_1- \underline P_0)= \\\big((1-t) x_0 + t x_1, (1-t )y_0 + t y_1\big)$ è la retta in $\mathbb{R}^2$ passante per i punti $\underline P_0,\underline P_1$.

$$
\underline P_t = (x,y)
$$

$$
\begin{cases}x = (1-t) x_0 + t x_1\\ y = (1-t )y_0 + t y_1\end{cases}
$$

Risolvendo in $t$ entrambe le equazioni otteniamo che $\frac{x-x_0}{x_1-x_0}=t=\frac{y-y_0}{y_1-y_0}$, cioè
$y = \frac{y_1-y_0}{x_1-x_0}(x-x_0)+y_0$.

Per $t\in [0,1]$, $P_t=(1-t)\underline P_0 + t\underline P_1$ è il segmento di estremi $\underline P_0,\underline P_1$, orientato da $\underline P_0 \text { a }\underline P_1$.

In generale, se $\underline P_0,\underline P_1 \in \mathbb{R}^n$, con $n\ge2$, l’espressione descriverebbe per $t\in \mathbb{R}$ la retta passante per i due punti.


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**

Se $f:I \subseteq \mathbb{R}\to \mathbb{R}$, con $I$  intervallo, $f$ è convessa in $I$  se e solo se $\forall x_0,x_1\in I$  e $\forall t\in [0,1]$ vale che $f(tx_1+(1-t)x_0)\le tf(x_1)+(1-t)f(x_0)$, da definizione.

Se $\underline P_0$ e $\underline P_1$ sono due punti distinti che giacciono sul grafico di $f$, il segmento di estremi $\underline P_0, \underline P_1$ è dato da
$P_t=(1-t)\underline P_0 + t\underline P_1=\big((1-t) x_0 + t x_1, (1-t )y_0 + t y_1\big)= (x_t,y_t)$.

Con questa notazione, la definizione di convessità diventa $f(x_t) \le y_t,\forall t\in [0,1]$, cioè all’ascissa $x_t$ il valore $f(x_t)$ è minore o uguale a $y_t$, cioè il punto $(x_t,f(x_t))$ giace sotto il punto $(x_t,y_t)$.

Possiamo anche scrivere - per quanto riguarda $\mathbb{R}^2$ - che
$f(x) \le \frac{f(x_1)-f(x_0)}{x_1-x_0}(x-x_0)+f(x_0), \forall x\in [x_0,x_1]$, ossia la funzione giace sotto la retta passante per i punti $(x_1, f(x_1))$ e $(x_2, f(x_2))$.

Equivalentemente possiamo dire che la corda di estremi $\underline P_0, \underline P_1$ giace sopra il grafico di $f$ tra $x_0$  e $x_1$.


# 1. Teoremi sulla concavità
>Teorema
> **Sia $f:I \subseteq \mathbb{R}\to \mathbb{R}$, con $I$  intervallo, tale che $f$ sia convessa in $I$. Allora $f$ è continua in $I$, salvo al più gli estremi di $I$. Inoltre essa possiede derivata destra e sinistra in ogni punto dell’intervallo, salvo al più gli estremi di $I$.**
> 

>Teorema
> **Sia $f:I \subseteq \mathbb{R}\to \mathbb{R}$, con $I$  intervallo, derivabile in $I$. Allora $f$ è convessa in $I$ se e solo se $f(x) > f(x_0)+f'(x_0)(x-x_0), \forall x\in I, \forall x_0 \in I$, cioè $f$ giace interamente sopra la tangente al suo grafico in $P_o(x_0, f(x_0)), \forall x_0\in I$.**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
$f= |x|$ è convessa anche se non è derivabile in tutto $\mathbb{R}$


![image.png](19%20Convessit%C3%A0%20e%20concavit%C3%A0/image.png)

>Teorema
> **Sia $f:I \subseteq \mathbb{R}\to \mathbb{R}$, con $I$  intervallo.**
> 
> 1. **Se $f$ è derivabile in $I$ , allora $f$ è convessa in $I$ se e solo se $f'$ è monotona crescente in $I$.**
> 2. **Se $f$ è derivabile due volte in $I$ , allora $f$ è convessa in $I$ se e solo se $f''(x)>0, \forall x \in I$.**

# 2. Punti di flesso e cambi di concavità

>Definizione: Punto di flesso
>**Data una funzione $f:(a,b) \to \mathbb{R}$ derivabile in $x_0$, con $x_0\in (a,b)$ , chiameremo $x_0$ punto di flesso per $f$ se 
$\exists \delta >0: f(x)\ge f(x_0)+f'(x_0)(x-x_0), \forall x \in [x_0,x_0+\delta)$ e se 
$f(x)\le f(x_0)+f'(x_0)(x-x_0), \forall x \in (x_0-\delta,x_0]$
oppure se 
$\exists \delta >0: f(x)\le f(x_0)+f'(x_0)(x-x_0), \forall x \in [x_0,x_0+\delta)$ e se 
$f(x)\ge f(x_0)+f'(x_0)(x-x_0), \forall x \in (x_0-\delta,x_0]$**


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Con abuso di notazione, per estensione, se $f$ è continua in $x_0$ e $f'(x_0)=\pm \infty$, con retta tangente verticale $x=x_0$, diremo ancora che $x_0$ è **punto di flesso, a tangente verticale.**


![image.png](19%20Convessit%C3%A0%20e%20concavit%C3%A0/image%201.png)

>Definizione: Cambio di concavità 
>**Data una funzione $f:(a,b) \to \mathbb{R}$ diremo che $x_0\in (a,b)$ è punto di cambio di concavità per $f$ se $\exists\delta >0$ tale che $f$ sia convessa (o concava) in $[x,x_0+\delta)$ e concava (o convessa, rispettivamente) in $(x_0-\delta,x_0]$.**


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Se $f:(a,b) \to \mathbb{R}$ è derivabile almeno una volta in $x_0$ e $x_0$ è punto di cambio di concavità, allora $x_0$   è punto di flesso.



>Teorema
> **Siano $f:(a,b) \to \mathbb{R}$ e $x_0\in(a,b)$. Se $f$ è derivabile due volte in $x_0$ e $x_0$ è punto di flesso per $f$, allora $f''(x_0)=0$.**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione** $x_0$  punto di flesso $\mathbb{R}ightarrow$  $f''(x_0) = 0$
$f''(x_0) = 0\mathbb{N}Rightarrow$ $x_0$  punto di flesso

Un esempio può essere la funzione $f(x) = x^4$, convessa in tutto $\mathbb{R}$, con derivata seconda che si annulla in $x=0$, ma che non può essere punto di flesso essendo minimo assoluto della funzione.


![image.png](19%20Convessit%C3%A0%20e%20concavit%C3%A0/image%202.png)

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Esistono funzioni non derivabili due volte in $x_0$ che hanno in $x_0$ un punto di flesso. Un esempio può essere la funzione $x^{5\over 3}$, la cui derivata seconda non esiste per $x= 0$, ma che ha in $x=0$ un punto di flesso.


![image.png](19%20Convessit%C3%A0%20e%20concavit%C3%A0/image%203.png)