# 3. Campi, insiemistica e intervalli

Tags: Insiemi numerici
Data lezione: 19/09/2024

# 1. Campi

> Definizione: Campo\
> **Ogni insieme $X$ dotato di due operazioni che soddisfano le proprietà di somma e prodotto viste nel paragrafo 2 del capitolo [1. Introduzione: insiemi numerici, logica e quantificatori](1%20Introduzione%20insiemi%20numerici,%20logica%20e%20quantifi%208086083780cf49709b466f3c30350a75.md) si dice campo. $\R, \, \mathbb{Q}, \, \mathbb{C}$ sono tutti campi.**
> 
>**Se $X$ è un insieme dotato di operazioni con tutte le proprietà di somma e prodotto e con relazione di ordine, allora si dice che $X$ è un campo ordinato. $\mathbb{Q}$ e $\R$ sono campi ordinati.**

Tutte le familiari regole di calcolo che utilizziamo abitualmente in $\R$ e in $\mathbb{Q}$ possono essere dedotte dagli assiomi di campo ordinato.

- $a \cdot 0 = 0, \, \forall a \in X$
- $-a = -1 \cdot a, \, \forall a \in X$
- $a^2 \ge 0, \forall a \in X$

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**\
Dall’ultima affermazione si può dedurre che in un campo ordinato vale la proprietà $a^2 +1 \ge 1>0, \, \forall a$; poiché in $\mathbb{C}$ abbiamo $i^2 +1 = 0$, $\mathbb{C}$ non può essere reso campo ordinato.



# 2. Numeri reali $\R$ e numeri razionali $\mathbb{Q}$ a confronto

Qual è il motivo per cui $\R$ è preferibile a $\mathbb{Q}$ per lo sviluppo dell’analisi matematica, nonostante, come visto al punto 2 di [1. Introduzione: insiemi numerici, logica e quantificatori](1%20Introduzione%20insiemi%20numerici,%20logica%20e%20quantifi%208086083780cf49709b466f3c30350a75.md) i due appaino dotati di proprietà simili e - come appena visto - entrambi siano campi ordinati? La risposta sta nel fatto che il primo soddisfa l’**assioma di continuità** mentre il secondo no - $\R$ è di fatto **l’unico** insieme ordinato a soddisfarlo.

Una delle forme dell’assioma di continuità è l’**assioma del $\sup$**, la proprietà dell’estremo superiore, che è trattata nel paragrafo 4 di questo capitolo.

# 3. Insiemi limitati, massimo e minimo, maggioranti e minoranti, estremo superiore ed estremo inferiore

Sia $X = \R\, o  \, X = \mathbb{Q}$ e consideriamo sottoinsiemi non vuoti $E \subseteq X$.

## 3.1 Insiemi limitati


>Definizione: Insiemi limitati\
>**Dato un sottoinsieme non vuoto $E \subseteq X$, esso si dice limitato superiormente (o dall’alto) se $\exists M\in X: x \le M,\, \forall x\in E$**
>
>**Dato un sottoinsieme non vuoto $E \subseteq X$, esso si dice limitato inferiormente (o dal basso) se  $\exists m\in X: m \le x,\, \forall x\in E$**
>
>**Un insieme è detto limitato se è limitato sia dal basso che dall’alto. $\exists m, M\in X: m \le x \le M,\, \forall x\in E$**

## 3.2 Massimo e minimo

>Definizione: Massimo\
>**Dato $E \subseteq X$ non vuoto, $x^* \in X$ si dice massimo di $E$ ($x^* = \max{E}$) se**
>1. $x^* \in E$
>2. $x \le x^*, \, \forall x \in E$

>Definizione: Minimo\
>**Dato $E \subseteq X$ non vuoto, $x_* \in X$ si dice minimo di $E$  ($x_* = \min{E}$) se**
>1. $x_* \in E$
>2. $x_* \le x, \, \forall x \in E$

Condizione necessaria, ma non sufficiente, affinché esista massimo o minimo è che l’insieme sia limitato dal lato giusto.

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**\
Non sempre esistono $\max{E}$ o $\min{E}$, anche se $E$ è limitato.

$E = \{  \frac{1}{n} : n \in \mathbb{N}, n\ge1\}$  è limitato superiormente e inferiormente, pur non avendo un minimo. Infatti $\max{E} = 1$, mentre inferiormente la sequenza tende a 0, senza mai giungerci. 

## 3.3 Maggioranti e minoranti

>Definizione: maggiorante\
>**Dato $E \subseteq X$ non vuoto, $k \in X$ (quindi non necessariamente $k \in E$) si dice maggiorante di $E$ se 
$x \le k\, \forall x \in E$**

> Definizione: minorante\
>**Dato $E \subseteq X$ non vuoto, $h \in X$ (quindi non necessariamente $k \in E$) si dice minorante di $E$ se 
$h \le x\, \forall x \in E$**

Se $k$  è maggiorante di $E$, anche ogni $a \gt k$ sarà maggiorante di $E$. Lo stesso ragionamento può essere fatto anche per i minoranti, a segno invertito. Maggioranti e minoranti esistono unicamente se l’insieme è limitato dal lato giusto.

Se $k$ è maggiorante di $E$ e $k \in E$, $\Rightarrow$ $k = \max{E}$

Se $h$ è minorante di $E$ e $k \in E$, $\Rightarrow$ $h = \min{E}$

### Esempi

- In $E = \mathbb{N}$ ogni $k \le 0$ è minorate, ma non esistono maggioranti.
- In $E = \{  \frac{1}{n} : n \in \mathbb{N}, n\ge1\}$   ogni $h \le 0$  è minorante, ogni $k \ge 1$ è maggiorante.
- In $E = \{ r \in \mathbb{Q} : r \ge 0, r^2 \le 2\} \sub \R$ ogni $h \le 0$  è minorante, ogni $k \ge \sqrt{2}$ è maggiorante.

## 3.4 Estremi superiore ed inferiore

>Definizione: estremi\
>**Sia $E \subseteq X$ non vuoto, se $E$ è limitato superiormente, chiamiamo estremo superiore ($\sup{E}$) il minimo dei maggioranti.**\
>
>**Sia $E \subseteq X$ non vuoto, se $E$ è limitato inferiormente, chiamiamo estremo inferiore ($\inf{E}$) il massimo dei minoranti.**



Il $\sup{E}$ è il migliore dei maggioranti, il più piccolo; l’$\inf{E}$ è il migliore tra i minoranti, il più grande.

### 3.4.1 Definizione matematica di estremo superiore ed estremo inferiore

**Dato $E \subseteq \R$ non vuoto e limitato dall’alto, $M \in \R$ è l’estremo superiore se:** 

- **$\forall x \in E, x \le M$**
- **$\forall k < M, \exists x \in E : k < x \le M$ o equivalentemente $\forall \epsilon > 0\exists x_0 \in E : x_0 > M-\epsilon$**



**Dato $E \subseteq \R$ non vuoto e limitato dal basso, $m \in \R$ è l’estremo inferiore se:** 

- **$\forall x \in E, m \le x$**
- **$\forall h > m, \exists x \in E : m<x <h$ o equivalentemente $\forall \epsilon > 0\exists x_0 \in E : x_0 < m+\epsilon$**


### Esempi

$E = \mathbb{N}$ 
$\nexists\sup{E}$
$\min{E} = \inf{E} = 0$

$E = \{  \frac{1}{n} : n \in \mathbb{N}, n\ge1\}$ 
$\max{E} = \sup{E} = 1$
$\nexists \min{E}$
$\inf{E} = 0$

# 4. Proprietà del $\sup$ e dell’$\inf$

> **$X$ soddisfa la proprietà dell’estremo superiore** (detta anche assioma di *Dedekind* **) se ogni sottoinsieme non vuoto $E \subset X$e limitato dall’alto possiede $\sup{E} \in X$**
> 

> **$X$ soddisfa la proprietà dell’estremo inferiore se ogni sottoinsieme non vuoto $E \subset X$ e limitato dal basso se possiede $\inf{E} \in X$**
> 

### Esempi

$E = \{ r \in \mathbb{Q} : r \ge 0, r^2 \le 2\} \subseteq \mathbb{Q}$
$\inf{E} = \min{E} = 0$
$\nexists \sup{E}$
$\nexists\max{E}$ 

$E = \{ r \in \mathbb{Q} : r \ge 0, r^2 \le 2\} \subseteq \R$
$\inf{E} = \min{E} = 0$
$\sup{E} = \sqrt{2}$
$\nexists\max{E} \Leftarrow \sqrt{2} \notin \mathbb{Q}$  

## 4.1 Corollari derivati dalla proprietà dell’estremo superiore


> Dato $E \subseteq \R$ non vuoto, se esiste $\max{E}$ o $\min{E}$ allora $\max{E} = \sup{E}$ o $\min{E} = \inf{E}$

>Se  $\sup{E} \in E$, $\Rightarrow$ $\sup{E} = \max{E}$ e parimenti se $\inf{E} \in E \Rightarrow \sup{E} = \min{E}$

> Dato $E \subseteq \R$ non vuoto e limitato dall’alto o dal basso, $\sup{E}$ o $\inf{E}$ esiste in $\R$.


## 4.2 Assioma di continuità di $\R$


**La proprietà dell’estremo superiore di $\R$ nella definizione assiomatica di $\R$ prende il nome di assioma di continuità di $\R$.**

> Definizione assiomatica di $\R$
> **Chiamiamo $\R$ un insieme che soddisfa le proprietà di somma, prodotto, relazione di ordine totale e dell’estremo superiore, ossia un campo ordinato che ha la proprietà dell’estremo superiore.** \
**[Analisi I - Bramanti, Pagani, Salsa]**


### 4.2.1 Corollari derivati dall’assioma di continuità di $\R$

> **Corollario**
> Dato $E \subseteq \R$ non vuoto, se $E$  è illimitato dall’alto, diremo che $\sup{E}= +\infty$

> **Corollario**
> Dato $E \subseteq \R$ non vuoto, se $E$ è illimitato dal basso, diremo che $\sup{E}= -\infty$

> **Corollario**
> Dato $E \subseteq \R$ non vuoto, esistono sempre $\sup{E}$ e $\inf{E}$


# 5. Modulo, disuguaglianza triangolare e retta dei numeri reali

>Definizione: Modulo\
>**Si dice valore assoluto o modulo di $a \in \R$ il numero ≥ 0 definito da $|a| = \begin{cases} a, & a\ge0 \\ -a, &a < 0 \end{cases}$**


**$\forall x,y \in \R$ vale la proprietà $|x+y| \le |x| + |y|$, che prende il nome di disuguaglianza triangolare.**

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**\
Spesso la disuguaglianza triangolare compare nella forma
$|a-b| \le |a-c| + |c-b|, \, \forall a,b,c, \in \R$, ottenuta per $x = a-c$ e $y = c-b$ 

## 5.1 La retta dei numeri reali

$\R$ può essere rappresentato geometricamente mettendolo in corrispondenza biunivoca con i punti di una retta orientata - e la stessa cosa potrebbe essere fatta anche per $\mathbb{Q}$, solo che la corrispondenza non sarebbe più biunivoca.

> Definizione: Corrispondenza biunivoca
>**La corrispondenza è biunivoca se ad ogni numero reale corrisponde uno ed un solo punto sulla retta e viceversa.**

Come si può notare nella definizione di corrispondenza biunivoca, per $\mathbb{Q}$ non è verificata l’ultima parte.


Per realizzare la retta dei numeri:

1. Si fissa arbitrariamente un punto sulla retta cui si associa $0$;
2. Si fissa arbitrariamente un secondo punto diverso dal primo cui si associa  $1$;
3. $\overline{01}$ è l’unità di misura;
4. Ad ogni $a \in \R$ si associa il punto sulla retta che è secondo estremo di un segmento avente primo estremo O e lunghezza $|a|$. Il punto è dallo stesso lato di 1 se $a >0$ , dal lato opposto se $a <0$.
    
    ![Line of real numbers](3%20Campi,%20insiemistica%20e%20intervalli/Real_number_line.svg)
    
    Line of real numbers
    


Geometricamente $|a|$ è la lunghezza del segmento di estremi $\overline{OA}$, ossia la distanze da $O$ ad $A$ Più in generale $|a-b|$ è la lunghezza del segmento di estremi $\overline{AB}$, cioè la distanza da $A$ a $B$, $\forall a,b \in \R$.

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Esistono punti sulla retta cui non corrisponde alcun punto $r\in\mathbb{Q}$. Un esempio potrebbe essere la $\sqrt{2}$.



![$\sqrt{2}$ on the line of real numbers](3%20Campi,%20insiemistica%20e%20intervalli/image.png)

$\sqrt{2}$ on the line of real numbers

# 6. Intervalli nella retta reale

## 6.1 Intervalli limitati

Dati $a,b \in \R, a<b$:

$(a,b) = \{x \in \R : a<x<b\}$

$(a,b] = \{x \in \R : a<x \le b\}$

$[a,b) = \{x \in \R : a\le x < b\}$

$[a,b] = \{x \in \R : a\le x \le b\}$

Tutti i precedenti sono **insiemi limitati**, tutti hanno $\inf = a$ e $\sup = b$; per gli insiemi in cui $a$ e $b$ sono contenuti, essi sono anche rispettivamente $\min$ e $\max$.

$(a,b)$ si dice **aperto**, $[a,b]$ **chiuso**; tuti i rimanenti non sono **né aperti né chiusi**.

## 6.2 Intervalli illimitati

Dati $a,b \in \R$:

$(a,+\infty) = \{x \in \R : a<x\}$

$[-\infty,b) = \{x \in \R : x < b\}$

$[a,+\infty) = \{x \in \R : a\le x\}$

$(-\infty,b] = \{x \in \R : x \le b\}$

Tutti i precedenti sono **insiemi illimitati o dall’alto o dal basso**; per quelli limitati dal basso si ha $\inf = a$, mentre per quelli limitati dall’alto si ha $\sup = b$; per gli insiemi in cui $a$ e $b$ sono contenuti, essi sono anche rispettivamente $\min$ e $\max$.

$(-\infty,b)$ e $(a, +\infty)$ si dicono **aperti**, $(-\infty,b]$ e $[a, +\infty)$ **chiusi**; tuti i rimanenti non sono **né aperti né chiusi**.

## 6.3 Intervallo illimitato dall’alto e dal basso

$(-\infty,+\infty) = \R$ è un **intervallo illimitato** e si dice che esso è **sia aperto che chiuso**.

# 7. Densità

> Definizone: Densità
>**$\forall x, y \in \R: x < y, \, \exists r \in \mathbb{Q} : x < r<y$**
**Si dice pertanto che $\mathbb{Q}$ è denso in $\R$.**

Ossia tra due numeri reali c’è un razionale e tra due razionali c’è un reale.