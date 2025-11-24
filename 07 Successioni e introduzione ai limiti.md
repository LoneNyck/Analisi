# 7. Successioni e introduzione ai limiti

Tags: Dimostrazione importante, Limiti, Successioni
Data lezione: 02/10/2024

# 1. Definizione di successione

> Definizione: Successione
>**Una funzione $f: \mathbb{N} \to \R$ si chiama successione di numeri reali.**

Più in generale si parla di successioni anche quando $f: A\subseteq \mathbb{N} \to \R$, con $A = \{n\in \mathbb{N}: n\ge n_0 \}$ per qualche $n_o \in \mathbb{N}$.

Spesso è usata la notazione $a_n, \{a_{n}\}, \{a_{n}\}_{n \ge n_0}$ invece di $f(n)$.

Il grafico di una successione è dato da una sequenza di **punti** in $\R^2$.

## 1.1 Successioni limitate

Come già visto al paragrafo 5 di [6. Nozioni elementari sulle funzioni](6%20Nozioni%20elementari%20sulle%20funzioni%2011034a78851580bf8b22e74f29991a40.md), anche le successioni essendo funzioni possono essere **limitate**.

- Se $\exists M \in \R: a_n\le M , \forall n\in \mathbb{N}$ allora la successione è detta **limitata dall’alto**;
- Se $\exists m \in \R: a_n\ge m , \forall n\in \mathbb{N}$ allora la successione è detta **limitata dal basso**;
- Se $\exists m,M \in \R: m\le a_n\le M , \forall n\in \mathbb{N}$ allora la successione è detta **limitata**;

## 1.2 Successioni monotone

Ancora, come per le funzioni del capitolo precedente, anche le successioni possono essere **monotone**. In particolare si dirà che una funzione è monotona:

- **crescente** se $a_n \le a_{n+1} \forall n\in \mathbb{N}$
- **strettamente crescente** se $a_n < a_{n+1} \forall n\in \mathbb{N}$
- **decrescente** se $a_n \ge a_{n+1} \forall n\in \mathbb{N}$
- **strettamente** **decrescente** se $a_n > a_{n+1} \forall n\in \mathbb{N}$

# 2. Limiti

## 2.1 Definizione di definitivamente

>Definizione: Definitivamente
>**Diremo che una successione $a_n$ soddisfa una proprietà $p$ definitivamente se $\exists N\in \mathbb{N} : a_n$ soddisfi $p, \forall n > N$.** 

## 2.2 Successioni convergenti e definizione di limite di successione

>Definizione: Limite e convergenza
>**Diremo che una successione converge ad un numero reale $\ell\in\R$ e scriveremo $\lim_{n\to\infty}a_n = \ell$ se 
$$\forall \epsilon >0\exists N\in \mathbb{N}: \forall n > N ,|a_n -\ell| < \epsilon$$ (o equivalentemente $\ell-\epsilon < a_n<\ell+\epsilon$).**

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**

$$
\lim_{n\to\infty}a_n = \ell \Leftrightarrow |\lim_{n\to\infty}a_n-\ell| = 0 \Leftrightarrow \lim_{n\to\infty}a_n-\ell = 0
$$

Non tutte le successioni ammettono un limite così definito.

## 2.3 Il teorema dell’unicità del limite
>Teorema: unicità del limite
> **Data una successione $a_n$, se $\exists \lim_{n\to\infty}a_n=\ell\in \R$, allora tale limite è unico.**
> 

### 2.3.1 Dimostrazione

Si tratta di una dimostrazione per assurdo, supponendo quindi che esitano due numeri $\ell_1 , \ell_2$ diversi tra loro -  supponendo il primo maggiore del secondo, - ambedue limiti di $f$. Si sceglie un $\epsilon< \frac{\ell_1-\ell_2}{2}$, in modo che $\ell_1 -\epsilon > \ell_2 + \epsilon$. Questo comporta che che tra $(\ell_1 -\epsilon; \ell_1 +\epsilon) \cap (\ell_2 -\epsilon; \ell_2 +\epsilon) = \empty$. Dalla definizione di limite segue che devono esistere dei numeri $N_1$ e $N_2$ : $\forall n>\max(N_1, N_2)$ $a_n \in (\ell_1 -\epsilon; \ell_1 +\epsilon) \cap (\ell_2 -\epsilon; \ell_2 +\epsilon)$, assurdo.

## 2.4 Successioni divergenti

> Definizione: Divergenza
>**Diremo che una successione diverge a $+\infty$ e scriveremo $\lim_{n\to\infty}a_n = +\infty$ se 
$$\forall M >0\exists N\in \mathbb{N}: \forall n > N, a_n>M$$** 
>
>**Diremo che una successione diverge a $-\infty$ e scriveremo $\lim_{n\to\infty}a_n = -\infty$ se 
$$\forall M >0\exists N\in \mathbb{N}: \forall n > N, a_n<-M$$** 

## 2.5 Estensione di $\R$ e successioni regolari e irregolari

> Definizione: $\R$ esteso
> **$\overline \R = \R^* = \R \cup \{\pm\infty\}$.**
> 

Data una successione $a_n$, se essa **converge oppure diverge**, allora diremo che $a_n$ è **regolare** e che $\exists \lim_{n\to\infty}a_n=\ell\in \overline\R$. Se invece la successione **non converge né diverge**, diremo che essa è **irregolare** (oppure **oscillante** oppure **indeterminata**) e che $\nexists \lim_{n\to\infty}a_n$.

## 2.6 Estensione del teorema dell’unicità del limite

Il teorema dell’unicità del limite visto al punto 2.3 di questo capitolo può essere esteso a tutto $\overline\R$.

>Teorema: unicità del limite in $\R$ esteso
> **Data una successione $a_n$, se $\exists \lim_{n\to\infty}a_n=\ell\in \overline\R$, allora tale limite è unico.**
> 

## 2.7 Infinitesimi e infiniti

>Definizione: Infiniti e Infinitesimi
>**Se $\lim_{n\to\infty}a_n = 0$ diremo che $a_n$ è infinitesima, mentre se $\lim_{n\to\infty}a_n = \infty$ diremo che essa è infinita.**

## 2.8 Convergenza per eccesso e per difetto

>Definizione: Convergenza per eccesso e difetto
**Diremo che $a_n$ converge per eccesso a $\ell\in \R$ se $\lim_{n\to\infty}a_n = \ell$ e $a_n \ge \ell$ definitivamente per $n\in \mathbb{N}$ e scriveremo $\lim_{n\to\infty}a_n = \ell^+$ se**
**$$\forall \epsilon >0\exists N\in \mathbb{N}: \forall n > N ,\ell<a_n<\ell+\epsilon$$** 
>
>**Diremo che $a_n$ converge per difetto a $\ell\in \R$ se $\lim_{n\to\infty}a_n = \ell$ e $a_n \le \ell$ definitivamente per $n\in \mathbb{N}$ e scriveremo $\lim_{n\to\infty}a_n = \ell^-$ se**
**$$\forall \epsilon >0\exists N\in \mathbb{N}: \forall n > N ,\ell-\epsilon<a_n<\ell$$ **

## 2.9 Teorema per successioni monotone

### 2.9.1 Teorema per successioni monotone e limitate

>Teorema
> **Sia $a_n$ una successione monotona e limitata. Allora 
$\exists \lim_{n\to\infty}a_n=\ell\in \R$.
Inoltre se $a_n$ è crescente $\ell = \sup a_n \in \R$ e $\lim_{n\to\infty}a_n= \ell^-$, mentre se  è decrescente $\ell = \inf a_n \in \R$ e $\lim_{n\to\infty}a_n= \ell^+$.**
> 

### 2.9.1 comma 1 - Dimostrazione

Prendiamo il caso in cui $a_n$ crescente.

Se $a_n$ è crescente e limitata per ipotesi significa che esisterà il $\sup$ di tale successione $\in \R$, che chiameremo $\ell$. Per la definizione di estremo superiore $a_n \le \ell, \forall n\in\mathbb{N}$ e $\forall \epsilon > 0 \exists n_0\in \mathbb{N}: \ell-\epsilon < a_{n_0} \le \ell$. Essendo $a_n$ crescente possiamo dedurre che $\forall n>n_0, a_n > a_{n_0}$. Queste condizioni unite permettono di affermare che $\forall \epsilon > 0 \exists n_0\in \mathbb{N}: \ell-\epsilon < a_{n} \le \ell\ \forall n> n_0$, che è la definizione di convergenza per difetto vista al punto 2.8 di questo capitolo.

---

Se $a_n$ cresce basta dire che essa e **limitata dall’alto**, in quanto necessariamente il primo termine sarà l’$\inf$, mentre se $a_n$  decresce sarà sufficiente dire che è **limitata dal basso,** in quanto il $\sup$ sarà il primo termine della sequenza.

### 2.9.2 Teorema per successioni monotone

Questo caso è una generalizzazione di quello appena visto, in quanto non è specificato se la funzione sia limitata o meno. Sta quindi a noi discutere i casi, facendo anche riferimento alla dimostrazione appena vista.
>Teorema
> **Sia $a_n$ una successione monotona. Allora essa ammette limite $\ell \in \overline \R.$
Inoltre se $a_n$ è crescente $\ell = \sup a_n \in \overline\R$, mentre se  è decrescente $\ell = \inf a_n \in \overline\R$.**
> 

### 2.9.2 comma 1 - Dimostrazione

Prendiamo ancora il caso in cui $a_n$ crescente.

1. Nel caso in cui $a_n$ fosse limitata, allora ci potremmo ricondurre alla dimostrazione vista al punto 2.9.1 comma 1. 
2. Nel caso in cui $a_n$ non fosse limitata, sapremmo comunque che essa è monotona crescente, da cui possiamo ricavare che $a_n > a_0$, $\forall n\in \mathbb{N}$. Dal fatto che essa non è limitata ricaviamo che il $\sup$ della successione è $+\infty$, che per definizione significa che $\forall M>0\exists n_0 \in \mathbb{N}: a_{n_0} > M$. Unendo le due condizioni ricaviamo che $\forall M>0\exists n_0 \in \mathbb{N}: a_n (\ge a_{n_0}) > M, \forall n\in \mathbb{N}$, che è proprio la definizione di $\lim$.



<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
$a_n$ monotona $\Rightarrow$ $a_n$ regolare, ma $a_n$ regolare $\nRightarrow$$a_n$ monotona

>Teorema
> **Data una successione $a_n$, se $\exists \lim_{n\to\infty}a_n=\ell\in \R$, allora essa è limitata.**
> 

## 2.10 Un particolare tipo di successione: la progressione geometrica

La progressione geometrica è una successione nella  $a_n = q^n, n\in \mathbb{N}$.

Il limite della progressione geometrica dipende dal valore della ragione $q$, infatti $\lim_{n\to\infty}q^n=$ 

- $+\infty$, se $q>1$
- $1$, se $q=1$
- $0$, se $|q|<1$

- $\nexists$ se  $q=-1$
- $\nexists$ se $q< -1$

## 2.11 Teoremi di permanenza del segno


>Teorema di permanenza del segno I
> **Data una successione $a_n$, se $\exists \lim_{n\to\infty}a_n=\ell\in \overline\R$ e $\ell>0$
$\Rightarrow$  $a_n > 0$ definitivamente in $n\in \mathbb{N}$. 
Similmente se $\ell<0$
$\Rightarrow$ $a_n < 0$ definitivamente in $n\in \mathbb{N}$.**
> 

### 2.11.1 - Dimostrazione

1. Se $\ell = +\infty$, per definizione di limite $a_n > M > 0$ definitivamente in $n\in \mathbb{N}$, quindi la dimostrazione si conclude qui in questo caso;
2. Se $\ell \in \R , \ell > 0$, nella definizione di limite adottiamo $\epsilon = \frac{\ell}{2}$ . Da questo ricaviamo che $a_n >  \ell - \epsilon = \frac{\ell}{2} > 0$ definitivamente in $n\in \mathbb{N}$.

---

Questo caso ribalta una parte dell’ipotesi con la tesi, rimuovendo però la maggioranza stretta - sul perché si vada all’osservazione in seguito alla dimostrazione.

>Teorema di permanenza del segno II
> **Data una successione $a_n$, se $\exists \lim_{n\to\infty}a_n=\ell\in \overline\R$ e $a_n \ge 0$ definitivamente in $n\in \mathbb{N}$ $\Rightarrow$  $\ell \ge 0$. 
Similmente se $a_n \le 0$ definitivamente in $n \in \mathbb{N}$ $\Rightarrow$  $\ell \le 0$.**
> 

### 2.11.2 - Dimostrazione

Cerchiamo di dimostrare per assurdo che $\ell < 0$. Per quanto dimostrato al punto 2.10.1, questo deve comportare che $a_n< 0$ definitivamente in $n\in \mathbb{N}$, assurdo e la dimostrazione si conclude qui. 

---

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Può essere che $\ell\ge0$ e $a_n <0$ $\forall n \in \mathbb{N}$, in quanto $\lim_{n\to\infty}a_n= 0$ $\ge 0$.
Parimenti se $a_n > 0$ $\forall n\in\mathbb{N}$ ed $\exists\lim_{n\to\infty}a_n$ $\Rightarrow$ $\ell\ge0$ e non $\ell>0$.
