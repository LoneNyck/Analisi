# 1. Introduzione: insiemi numerici, logica e quantificatori

Tags: Insiemi numerici\
Data lezione: 18/09/2024

# 1. Insiemi numerici

## 1.1 I numeri naturali $\mathbb{N}$

$\mathbb{N}$  è l’insieme dei numeri naturali e comprende tutti i **numeri interi non negativi**. La sua rappresentazione per elencazione è $\mathbb{N} = \{0,1,2,...\}$

## 1.2 I numeri relativi $\mathbb{Z}$

$\mathbb{Z}$ è l’insieme di numeri relativi e comprende tutti i **numeri interi, positivi o negativi** che siano. La sua rappresentazione per elencazione è 
$\mathbb{Z} = \{...,-3,-2,-1,0,1,2,3,...\}$

## 1.3 I numeri razionali $\mathbb{Q}$

$\mathbb{Q}$ è l’insieme dei numeri razionali e comprende tutte le **multiple frazioni equivalenti**. La sua rappresentazione è $\mathbb{Q} = \{ \frac{m}{n}:m,n \in \mathbb{Z}, n \neq 0\}$

Due frazioni sono tra loro equivalenti se $\frac{m}{n} = \frac{a}{b} \Leftrightarrow ma=nb, b\neq 0.$

Ogni numero $r\in\mathbb{Q}$ può anche essere espresso sotto forma di numero decimale. In tal maniera l’insieme dei numeri razionali può anche essere scritto come 
$\mathbb{Q} = \{ r= \pm a_0,a_1a_2...a_k, a_0\in\mathbb{N}, a_k\in\{0,1,...,9\} \forall k \in \mathbb{N}, k\neq 0 \text{ e la rappresentazione decimale sia finita o infinita e periodica}\}$

Quest’ultima definizione fa notare come nell’insieme dei razionali manchino tutti quei numeri con espansione decimale infinita e non periodica, quali $\pi$, $\sqrt{2}$,…


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione** \
All’interno di $\mathbb{Q}$ la rappresentazione decimale non è unica.
Un esempio può essere costituito dal caso $0,\bar9 = 1$


## 1.4 I numeri reali $\mathbb{R}$

L’insieme dei numeri reali è definito come 
$\mathbb{R} = \{r=\pm a_0,a_1a_2...a_k, a_0\in\mathbb{N}, a_k\in\{0,1,...,9\} \forall k \in \mathbb{N}, k\neq 0\}$ 
e contiene **tutti i numeri che hanno rappresentazione decimale finita, infinita e periodica e infinita e non periodica.**

I numeri che appartengono all’insieme $\mathbb{R} \setminus\mathbb{Q} = r\in\mathbb{R}:r\notin \mathbb{Q}$ sono detti **irrazionali** e fanno parte di questa categoria di numeri $\pi$, $\sqrt{2}$, $\sqrt{3}$,…

## 1.5 I numeri complessi $\mathbb{C}$

L’insieme dei numeri complessi è definito come $\mathbb{C} = \{z = a+bi:a,b\in\mathbb{R}, i^2 = -1\}$ [vedi [5. Numeri complessi](5%20Numeri%20complessi%2010c34a788515800ea48ac9acd1bbe90a.md) per il capitolo dedicato ai numeri complessi].

![Venn diagram of Numbers](1%20Introduzione%20insiemi%20numerici,%20logica%20e%20quantifi/Venn_Diagram_of_Numbers_Expanded.svg)

Venn diagram of Numbers

---

I vari insiemi numerici possono essere **ordinati** nel seguente modo sfruttando le relazioni tra insiemi: 
$\mathbb{N} \sub \mathbb{Z} \sub \mathbb{Q} \sub \mathbb{R} \sub \mathbb{C}$

# 2. Operazioni in $\mathbb{R}$ e in $\mathbb{Q}$

In $\mathbb{R}$ e $\mathbb{Q}$ sono definite due operazioni - **somma** e **prodotto** (e le relative inverse, rispettivamente differenza e divisione) - con le seguenti proprietà:

### Somma

- Proprietà commutativa:
$a+b = b+a,  \forall a,b$
- Proprietà associativa:
$(a+b)+c=a+(b+c),  \forall a,b,c,$
- Elemento neutro:
$a+0=a, \forall a$
- Elemento opposto:
$a+(-a) = 0, \forall a$

### Prodotto

- Proprietà commutativa:
$a\times b = b \times a,  \forall a,b$
- Proprietà associativa:
$(a \times b) \times c=a \times(b \times c),  \forall a,b,c,$
- Elemento neutro:
$a \times 1 = a, \forall a$
- Elemento inverso:
$a \times a^{-1} = 1, \forall a \ne 0$ 
con $a^{-1} = {1 \over a}$

Esiste poi la proprietà distributiva, che si applica quando somma e prodotto interagiscono reciprocamente.

$(a+b)c = ac+bc$

I due insieme sono anche caratterizzati dalla proprietà di essere ordinabili. In $\mathbb{R}$ e in $\mathbb{Q}$ è definita una **relazione d’ordine totale:** ciò significa che ogni elemento del campo [per la definizione di campo vai a [3. Campi, insiemistica e intervalli](3%20Campi,%20insiemistica%20e%20intervalli%20eb86f163c8994969a366838e8e38ffc6.md), par.1] può essere confrontato con un altro elemento dello stesso campo. La relazione d’ordine ha le seguenti proprietà:

- Riflessività: $a \le a, \forall a$
- Antisimmetria: $a \le b \, e \, b\le a \Rightarrow a = b$
- Transitività: $\forall a, b, c, \, se \, a\le b\le c \Rightarrow a\le c$
- Totale: $\forall a, b, $ vale $a\le b$ o $b\le a$

Inoltre valgono le seguenti proprietà:

- $\forall a,b,c, \, a \le b\Rightarrow a+c \le b+c$
- $\forall a,b \, e \, \forall c>0, \, a<b \Rightarrow ac<bc$

# 3. Elementi base di logica

> Definizione: Proposizione\
>**Una proposizione è un enunciato non contenente variabili libere cui si possa attribuire il valore vero o falso (solo uno dei due) in maniera univoca.**

> Definizione: Predicato\
> **Si definisce predicato un enunciato contenente variabili libere il cui valore di verità dipenda dal valore delle variabili. Per ogni assegnazione della variabile il predicato deve essere o vero o falso, non entrambi,**

Le proposizioni si indicano utilizzando lettere latine maiuscole $P, Q,...$ mentre i predicati si indicano con lettere latine maiuscole seguite dalle variabili $P(x,y,...), Q(n),...$

# 4. Connettivi logici

>**$\land$ corrisponde alla ‘e, logica**

Date $P$ e $Q$, $P\wedge Q$ è la proposizione vera se sono vere entrambe, falsa altrimenti

>**$\lor$ corrisponde alla ‘o, logica**

Date $P$ e $Q$, $P\vee Q$ è la proposizione vera se almeno una delle due è vera, falsa altrimenti

> **$\lnot$ corrosponde al ‘non, logico**

Data $P$, $\neg P$ è la proposizione vera se $P$ è falsa, falsa se $P$ è vera

> **$\implies$ corrisponde a ‘implica,**

Date $P$ e $Q$, $P\Rightarrow Q$ è la proposizione vera se $P$ è vera e $Q$  è vera o se $P$ è falsa e qualunque sia il valore di verità di $Q$ ; essa è falsa solo se $P$ è vera e $Q$ falsa

> **$\iff$ corrisonde a ‘se e solo se,**

Date $P$ e $Q$, $P\Leftrightarrow Q$ è la proposizione vera se $P$ e $Q$  sono ambedue vere o false, altrimenti è falsa.

# 5. Quantificatori

Al fine di stabilire il valore di verità di una proposizione è necessario attribuire alle variabili dei valori, saturandole. Ciò è fatto mediante l’utilizzo dei quantificatori.

> **I quantificatori sono:**
>- **$\forall$, che corrisponce a ‘per ogni’**
>- **$\exists$ che corrisponde a ‘esiste’**
>- **$\exists!$ che corrisponde a ‘esiste ed è unico’**
>- **$\nexists$ che corrisponde a ‘non esiste alcun’**

Dato $P(x), x\in A$:
- per $x=x_0:P(x)$
- $\forall x \in A:P(x)$
- $\exists x\in A:P(x)$
- $\exists! x \in A: P(x)$
- $\nexists x \in A: P(x)$

in generale sono proposizioni diverse.


>Definizoine: Implicazione Universale
>**Dato un insieme $A$ e i predicati $P(x), Q(x), x \in A$, si definisce implicazione universale la struttura $\forall x \in A , P(x) \Rightarrow Q(x)$.**


>Definizione: Condizione sufficiente e condizione necessaria\
>**Date $P, Q$, se $P \Rightarrow Q$, $P$ è condizione sufficiente affinché $Q$ e $Q$ è condizione necessaria affinché $P$.**

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**\
**Date $P, Q$, se $P \Leftrightarrow Q$ è vera, $P$ è condizione sufficiente e necessaria affinché $Q$ e viceversa.**