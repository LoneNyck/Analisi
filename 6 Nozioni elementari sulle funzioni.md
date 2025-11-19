# 6. Nozioni elementari sulle funzioni

Tags: Dimostrazione importante, Funzioni
Data lezione: 27/09/2024

# 1. Definizione di funzione, dominio, codomino e immagine

La funzione permette di descrivere matematicamente il concetto di grandezza variabile, che sottintende l’esistenza di una relazione tra grandezza, ossia la dipendenza di una rispetto all’altra.


> Definizione: Funzione, dominio, codominio
> **Dati due insiemi $A$ e $B$, una funzione $f:A \to B$ è una legge che associa a ciascun elemento $a \in A$ uno è un solo elemento $b \in B$. Scriveremo $y = f(x)$.**
>**$A$ prende il nome di dominio di $f$, $B$ di codominio di $f$**

>Definizione: immagine
> **Se $x \in A$, l’elemento $y= f(x) \in B$ si dice immagine di $x$ tramite $f$**
>$$
x \in A \to_f y = f(x) \in B
$$

>Insieme immagine
>**Si chiama immagine di $A$ tramite $f$ (o immagine di $f$) l’insieme
$Im_f = f(A) = \{ y \in B: \exists x \in A: f(x) = y \}$ degli elementi di $B$ che provengono da qualche elemento di $A$ tramite $f$.**


In generale $Im_f \subseteq B$, ma può accadere che $Im_f \sub B$.

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**

$f: \mathbb{R} \to \mathbb{R}$: $f(x) = x^2$

$f:\mathbb{R} \to [0,+\infty)$: $g(x) = x^2$

e $f: (-\infty; 0] \to [0,+\infty)$: $h(x) = x^2$

in generale sono funzioni diverse tra loro.


# 2. Suriettività

>Definizione: suriettività
>**Data $f: A\to B$, se $Im_f = B$, allora $f$ si dice suriettiva, ossia ad ogni elemento del codominio corrisponde almeno un elemento del dominio.**


# 3. Dominio e controimmagine

**Una funzione viene assegnata dichiarandone il dominio di $f: A \to B$ con $D_f = A$**


![image.png](6%20Nozioni%20elementari%20sulle%20funzioni/image.png)

>Definizione: controimmagine
>**Data $f:A\to B$, $C \subseteq B$, l’insieme $f^{-1}(c) = \{x \in A: f(x) \in C\} \subseteq A$ si dice controimmagine di $C$  tramite $f$.**

# 4. Grafico di una funzione

>Definizione: Grafico di una funzione
>**Il grafico di una funzione $f:A \to B$ è il sottoinsieme di $A\times B,$ definito come segue: 
$G_f = \{(x,y) \in (A\times B): x \in A, y = f(x) \in B \}$**


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Se $f: A\to B$ e $A,B \subseteq \mathbb{R}$ $\mathbb{R}ightarrow$ $G_f = \mathbb{R}^2$


Il fatto che $\forall x_0 \in A$ esiste **un’unica** **immagine** $y_0 \in B$, $A,B \subseteq \mathbb{R}$, si interpreta geometricamente nel grafico di $f$ osservando che ogni retta verticale lo interseca al più una volta; in particolare 0 volte se $x \mathbb{N}otin A$, 1 volta se $x \in A$. In quest’ultimo caso l’ordinata del punto sul grafico è $y = f(x_0)$. 

Il **dominio** della funzione non è altro che la **proiezione** del grafico sull’asse delle **ascisse**.

Inoltre $y_0 \in Im_f$ se e solo se esiste un punto $(x_0,y_0) \in G_f$ di ordinata $x_0$.

L’**insieme delle immagini** non è altro che la **proiezione** del grafico sull’asse delle **ordinate**. 

# 5. Funzioni limitate

>Definizione: funzione limitata
> **Data $f: A \subseteq \mathbb{R}\to \mathbb{R}$ diremo che:**
> **$f$ è limitata dall’alto se $\operatorname{Im}f \subseteq \mathbb{R}$ è limitato superiormente, cioè $\exists M\in \mathbb{R} : f(x) < M, \forall x \in A$**
> 
> **$f$ è limitata dal basso se $\operatorname{Im}f \subseteq \mathbb{R}$ è limitato inferiormente, cioè 
$\exists m\in \mathbb{R} : f(x) > m, \forall x \in A$**
>
> **$f$ è limitata se $\operatorname{Im}f\subseteq \mathbb{R}$ è limitato sia dall’alto che dal basso, cioè
$\exists m,M\in \mathbb{R} : m< f(x) < M, \forall x \in A$**
> 

Inoltre possiamo anche definire come per gli insiemi:

- $\sup f(x) = \sup \operatorname{Im}f$ **estremo superiore** di $f$
- $\inf f(x) = \inf \operatorname{Im}f$ **estremo inferiore** di $f$
- $\max f(x) = \max \operatorname{Im}f$ **massimo** di $f$
- $\min f(x) = \min \operatorname{Im}f$ **minimo** di $f$

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
$\sup f(x)$ e $\inf f(x)$ esistono sempre in $\mathbb{R} \cup\{\pm\infty\}$ e sono eventualmente infiniti. Inoltre se esistono massimo e minimo della funzione, allora essi coincidono con estremo superiore ed inferiore.

In molti casi una funzione reale in variabili reali viene assegnata solo mediante la sua espressione **analitica**, non dichiarando esplicitamente dominio o codominio; in generale il codominio sottinteso è $\mathbb{R}$ mentre il dominio corrisponde al più grande sottoinsieme $A \subseteq \mathbb{R}$ dove la regola analitica assegnata è ben definita e si parla in questo caso di **campo di esistenza**.

# 6. Funzioni pari e dispari, monotonia e periodicità

## 6.1 Simmetrie di una funzione

>Definzione: funzini pari e dispari
>**Dato $a >0, f: (-a,a) \subseteq \mathbb{R}\to \mathbb{R}$, con $a$  non necessariamente finito, $f$ si dice pari se vale $f(x) = f(-x), \forall x \in (a,-a)$. 
Si dirà invece dispari se vale $-f(x) = f(-x), \forall x \in (a,-a)$.
In caso nessuna condizione precedente sia soddisfatta, $f$ non sarà né pari né dispari.**

Le funzioni pari hanno grafico simmetrico rispetto a $x=0$; quelle dispari rispetto all’origine degli assi.

## 6.2 Monotonia

Sia data $f: A \subseteq \mathbb{R}\to \mathbb{R}$.

>Definizione: monotonia
> **Se $\forall x_1, x_2 \in A, x_1<x_2 \mathbb{R}ightarrow f(x_1)\le f(x_2)$ allora essa si dirà monotona crescente.**
>
>**Se $\forall x_1, x_2 \in A, x_1<x_2 \mathbb{R}ightarrow f(x_1)<f(x_2)$ allora essa si dirà monotona strettamente crescente.**
>
>**Se $\forall x_1, x_2 \in A, x_1<x_2 \mathbb{R}ightarrow f(x_1) \ge f(x_2)$ allora essa si dirà monotona decrescente.**
>
>**Se $\forall x_1, x_2 \in A, x_1<x_2 \mathbb{R}ightarrow f(x_1)> f(x_2)$ allora essa si dirà monotona strettamente decrescente.**

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Si noti che non è necessario che $f(x)$ sia continua per essere monotona.


Se $f$ è crescente, la disuguaglianza tra gli argomenti viene preservata, se $f$ è decrescente essa viene invertita.

![image.png](6%20Nozioni%20elementari%20sulle%20funzioni/image%201.png)

Un altro modo per verificare la crescenza di una funzione è l’uso del **rapporto incrementale**:

- ${f(x_2) - f(x_1) \over x_2 - x_1 } \ge 0, \forall x_1,x_2\in \operatorname{D}_f, x1 \mathbb{N}eq x_2$  $\mathbb{R}ightarrow$ $f$ è crescente
- ${f(x_2) - f(x_1) \over x_2 - x_1 } \le 0, \forall x_1,x_2\in \operatorname{D}_f, x1 \mathbb{N}eq x_2$  $\mathbb{R}ightarrow$ $f$ è decrescente

Inoltre una funzione del tipo $f(x) = k, k\in R$ si dice **sia crescente che decrescente**.

## 6.3 Periodicità

> Definizione: periodicità
>**Sia $f: A \subseteq \mathbb{R}\to \mathbb{R}$; diremo che si tratta di una funzione periodica di periodo $T$ se $f(x+T) = f(x), \forall x \in A$.
Ogni intervallo lungo $T$ contenuto in $A$ si chiama intervallo di periodicità.**


# 7. Composizione di funzioni

>Definizione: composizione di funzioni
>**Date due funzioni $f: A\to B$ e $g: B \to C$, $g \circ f$ prende il nome di funzione composta di $f$ e $g$ ed associa ad ogni elemento di $A$ uno e un solo elemento di $C$.**
> $$g \circ f: A \to C$$


È possibile comporre anche più funzioni e si dimostra che vale la proprietà **associativa**, ossia
$(h \circ g)\circ f = h \circ (g \circ f)$, ma in generale **non** vale quella **commutativa**, quindi
$g \circ f \mathbb{N}eq f \circ g$

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Non tutte le funzioni possono essere composte, in quanto potrebbero insorgere problemi di esistenza; un caso potrebbe essere $f(x) = -x^2$  e $g(t) = \log t$.


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Se $f: A\to B$ e $g: D \subseteq B \to C$ possiamo definire $g \circ f: \text{Dom}_f \to C$, $\text{Dom}_f = \{x\in A: f(x) \in D \} = A \cap f^{-1}(D) \subseteq A$. Un esempio è dato delle funzioni $f(x) = \sqrt{x}$, definita solo in $[0,+\infty),$ e $g(t) = t^2$, definita in tutto $\mathbb{R}$. La composizione tra le due sarà pertanto $g \circ f = x, x \ge 0$.

# 8. Iniettività e invertibilità

> **Data $f: A\to B$, se equivalentemente**
> 1. **$\forall x_1, x_2  \in A, x_1 \mathbb{N}eq x_2 \mathbb{R}ightarrow f(x_1) \mathbb{N}eq f(x_2)$**
> 2. $\forall x_1, x_2  \in A, f(x_1) = f(x_2)\mathbb{R}ightarrow x_1 = x_2$ 
> 3. $\forall y \in Im_f \exists! x\in A: f(x) = y$
>
>**allora $f$ è iniettiva.**

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazioni**

- Se $y \in \text{Im}_f \mathbb{R}ightarrow \exists x \in \text{Dom}_f : f(x) = y$  per definizione, mentre se 
$y \mathbb{N}otin Im_f \mathbb{R}ightarrow \mathbb{N}exists x \in Dom_f$  siffatta

Se $f$ è **suriettiva**, essa **ammette** **sempre** una **soluzione**  $x \in Dom_f$ $\forall y \in Im_f$; se $f$  è **iniettiva**, essa **può** **non** **avere soluzione**   $x \in Dom_f$ $\forall y \in Im_f$, ma quando quest’ultima esiste, allora è **necessariamente** **unica**.

>Definizione: Initettività
>**Data $f: A\to B$ iniettiva, la funzione che $\forall y \in Im_f$  associa l’unico $x \in A: f(x) = y$ si chiama funzione inversa di $f$ e si indica con 
$f^{-1}: Im_f\subseteq B\to A$.**


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazioni**

- $f^{-1}(f(x)) = x$
- $f(f^{-1}(y)) = y$

**Se $f$ è iniettiva, diremo allora che essa è invertibile sulla propria immagine, cioè $\exists f^{-1}:Im_f \subseteq B \to A$**

## 8.1 Teorema sulla monotonia e sull’invertibilità

>Teorema: monotonia e iniettività implicano invertibilità
> **$f: A\subseteq \mathbb{R} \to \mathbb{R}$ strettamente monotona in $A$ $\mathbb{R}ightarrow$ $f$  è iniettiva $\mathbb{R}ightarrow$ $f$ è invertibile.
Inoltre la funzione inversa sarà anch’essa strettamente monotona.**
> 

### 8.1.1 Dimostrazione

Per ogni coppia di $x_1, x_2$, la crescenza stretta impone che se la prima è minore della seconda, allora anche l’immagine della prima sarà minore di quella della seconda. Se le due ascisse sono tra loro diverse, senza ulteriori specificazioni, la monotonia stretta impone che una sia necessariamente maggiore dell’altra, il che conferma che $x_1 \mathbb{N}eq x_2$, dimostrando l’iniettività di di $f$.

La dimostrazione prosegue per assurdo, supponendo di avere una coppia di ordinate $y_1 < y_2$ tali che $f^{-1}(y_1) = x_1>f^{-1}(y_2)=x_2$. Se $x_1 > x_2$, essendo la funzione strettamente crescente, significa che $f(x_1)= y_1> f(x_2) = y_1$, assurdo. 

## 8.2 Considerazioni sull’invertibilità

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
**Esistono funzioni invertibili non monotone**, quindi è la monotonia stretta è condizione sufficiente ma non necessaria per l’invertibilità.


Calcolare analiticamente $f^{-1}(y), \forall y \in Im_f$   vuol dire risolvere l’equazione $f(x) = y$ in $x \in Dom_f ,\forall y \in Im_f$.

Data una funzione invertibile, il suo grafico si ottiene da quello della funzione di partenza per simmetria rispetto alla bisettrice di I e III quadrante, ossia rispetto a $y=x$.

![image.png](6%20Nozioni%20elementari%20sulle%20funzioni/image%202.png)