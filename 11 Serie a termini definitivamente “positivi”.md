# 11. Serie a termini definitivamente “positivi”

Tags: Serie
Data lezione: 17/10/2024

# 1. Definizione
>Definizione: Serie a termini positivi
>**Data la serie $\sum_{n=0}^{+\infty} a_n$ , essa si dice a termini “positivi” - o non negativi - se $a_n \ge 0$ definitivamente in $n\in \N$.**

# 2. Teorema della convergenza o divergenza per serie a termini positivi
>Teorema: Convergenza per serie a termini positivi
> **Se la serie $\sum_{n=0}^{+\infty} a_n$  è a termini positivi definitivamente in $n\in \N$, allora essa converge o diverge a $+\infty$.**
> 

## 2.1 Dimostrazione

L’idea della dimostrazione è mostrare che la successione delle somme parziali sia definitivamente crescente, ossia per il teorema di esistenza di successioni monotone [[7. Successioni e introduzione ai limiti](7%20Successioni%20e%20introduzione%20ai%20limiti%2011334a78851580b9b79fcb0887cf2531.md), par. 2.9.2] deve esistere il limite di $S_N \in \overline \R$, cioè $\sum_{n=0}^{+\infty} a_n = s \in \overline \R$. 

Per ipotesi $a_n$ è definitivamente positiva, ossia $\exist n_0 \in \N: \forall n \ge n_0$  $a_n\ge0$. Di conseguenza $\forall N \ge n_0$  $S_N = S_{N-1} + a_N \ge S_{N-1}$$\Rightarrow$ $S_N$ è definitivamente crescente.

# 3. Confronto per serie a termini positivi

>Teorema del confronto
> **Siano date le successioni $a_n$  e $b_n$  : $0\le a_n \le b_n$ definitivamente in $n\in \N$.**
> 
> 1. **Se $\sum_{n=0}^{+\infty} a_n$  diverge $\Rightarrow$ $\sum_{n=0}^{+\infty} b_n$  diverge;**
> 2. **Se $\sum_{n=0}^{+\infty} b_n$  converge $\Rightarrow$ $\sum_{n=0}^{+\infty} a_n$  converge;**
> 
> **Inoltre se $0\le a_n \le b_n, \forall n\in N$ $\Rightarrow$ $\sum_{n=0}^{+\infty} a_n \le \sum_{n=0}^{+\infty} b_n$** 
> 

## 3.1 Dimostrazione

Supponiamo che $0\le a_n\le b_n \forall n\in \N$.

Chiamiamo $S_N = \sum_{n=0}^{N} a_n$  e $\sigma_N = \sum_{n=0}^{N} b_n$ . Dalla condizione dell’ipotesi segue che $\sum_{n=0}^{N}a_n < \sum_{n=0}^{N}b_n$ ossia che $S_N <\sigma_N, \forall N\in \N$. 

Per il teorema visto al punto 2. di questo capitolo $S_N$ e $\sigma_N$ sono entrambe monotone crescenti. Questo significa che esistono i due limiti delle due somme parziali $\in \overline \R$, che chiameremo $s$  e $\sigma$. 

1. Se $\sum_{n=0}^{N}a_n$ diverge $\Rightarrow$  $s = +\infty$ ed essendo $S_N <\sigma_N, \forall N\in \N$, allora $s<\sigma$ 
$\Rightarrow \sigma = +\infty$ $\Rightarrow \sum_{n=0}^{N}b_n$ diverge.
2. Se $\sum_{n=0}^{N}b_n$ converge $\Rightarrow$  $\sigma \in \R$. $S_N \le \sigma_N \le \sigma$ $\Rightarrow S_N$ è crescente e limitata
$\Rightarrow \sum_{n=0}^{N}a_n$ converge

## 3.2 Alcune serie per svolgere il confronto

Le serie che seguono sono utili per effettuare i confronti con il teorema precedente al fine di stabilire il carattere di un’altra serie, essendo il loro carattere noto o ricavabile.

### 3.2.1 Serie geometrica

La serie **geometrica** già vista in [10. Serie di numeri reali](10%20Serie%20di%20numeri%20reali%2012134a7885158025ab5eda4c4a2cb72b.md), paragrafo 2. può essere utilizzata per effettuare il confronto, dipendendo il suo valore da quello della ragione $q$.

### 3.3.2 Serie armonica
>Teorema
> **La serie armonica $\sum_{n=1}^{+\infty}\frac{1}{n}$ diverge.**
> 

Si può dimostrare con il teorema del confronto che la serie armonica diverge. 

Per la definizione di numero di Nepero abbiamo che $e = \lim_{n\to \infty}(1+\frac1{n})^n= \sup (1+\frac1{n})^n$. Questo significa che $e \ge (1+\frac1{n})^n$. Svolgendo il logaritmo da ambedue le parti otteniamo che $1 \ge \log(1+\frac1{n})^n = n\log(1+\frac1{n})$.
$1/n \ge \log (\frac{n+1}{n})= \log (n+1)-\log n$. Notiamo che il termine a destra della disuguaglianza è nella forma $b_{n+1}-b_n =-(b_n-b_{n+1})$, ossia la sua serie è una serie telescopica, il cui valore sarà dato da $-(b_0-\lim_{n\to\infty}b_n) = -(0 - \infty) = +\infty$. Per il teorema del confronto $1\over n$  diverge.

### 3.3.3. Serie armonica generalizzata

La serie **armonica** può essere **generalizzata** per includere anche il caso di potenze e logaritmi al denominatore.

La serie $\sum_{n=0}^{+\infty}\frac{1}{(\log^\beta n) n^\alpha}:$

- **converge** per $\alpha > 1 \vee \forall \beta$ e per $\alpha = 1 \wedge \beta > 1$

- **diverge** per $\alpha < 1 \vee \forall \beta$ e per $\alpha = 1 \wedge \beta \le 1$

# 4. Confronto asintotico per serie
> Teorema: confronto asintotico per serie
> **Siano date le successioni $a_n$  e $b_n$  a termini definitivamente positivi e supponiamo che sia $a_n \sim b_n$ $\Leftrightarrow \lim_{n\to\infty} \frac{a_n}{b_n} = 1$. Allora $\sum_{n=0}^{+\infty} a_n$  e $\sum_{n=0}^{+\infty} b_n$  hanno lo stesso carattere, ossia o convergono o divergono a $+\infty$.**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Anche se $a_n$ e $b_n$  convergono entrambe, in generale il risultato delle due somme sarà diverso.


## 4.1. Dimostrazione

Per ipotesi sappiamo che il limite del rapporto delle due successione tende a 1. Nella definizione di limite adottiamo $\epsilon = \frac{1}{2}$. Allora per la definizione di limite avremo che$\exist N_1 \in \N: \forall n > N_1$ $1 -\epsilon < \frac{a_n}{b_n} < 1+\epsilon$ $\Rightarrow$ ${1\over 2} < \frac{a_n}{b_n} < {3\over 2}$. Essendo le due successioni definitivamente positive significa che $\exist N_2 \in \N: \forall n > N_2, a_n > 0, b_n >0$.

Questo implica che $\forall n> \max (N_1, N_2 )= N$

1. $0<a_n < {3\over 2}b_n$ 
2. $0< b_n < 2a_n$

Applicando quindi il teorema del confronto al caso i. segue che se la serie di $a_n$ diverge, allora anche quella di $b_n$ deve divergere, mentre se quella $b_n$  converge, allora anche la serie degli $a_n$ è costretta a convergere; dal caso ii. ricaviamo che se la serie di $b_n$  diverge, quella degli $a_n$ fa altrettanto, mentre se la serie di $a_n$ converge, allora convergerà anche quella di $b_n$.

# 5. Criterio del rapporto per serie e del criterio della radice

## **5.1 Criterio del rapporto per serie**
>Teorema: Criterio del rapporto per serie
> **Sia $a_n$ una successione di termini definitivamente positivi in $n \in \N$ e $\exist \lim_{n\to\infty}\frac{a_{n+1}}{a_n}= \ell\in \overline \R$. Allora se**
> 
> 1. **$\ell > 1\Rightarrow \sum_{n=0}^{+\infty} a_n$  diverge e  $\lim_{n\to\infty}{a_n}= +\infty$**
> 2. **$0\le \ell < 1\Rightarrow \sum_{n=0}^{+\infty} a_n$  converge e  $\lim_{n\to\infty}{a_n}= 0$**

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Se $\ell = 1$  non è possibile concludere nulla sul carattere della serie, in quanto esistono serie che convergono e serie che divergono per quel valore di $\ell$. 


### 5.1.1. Dimostrazione

Supponiamo $a_n > 0, \forall n \in \N$ e sia $\ell = \lim_{n \to \infty} \frac{a_{n+1}}{a_n}$.

1.  Assumiamo che sia $0\le \ell < 1$. Nella definizione di limite assumiamo $\epsilon = \frac{1-\ell}{2}$, da cui $\exist N \in \N :\forall n> N \, { a_{n+1}\over a_n} < \ell+\epsilon$. Questo significa che ${a_{n+1}\over a_n} < {1+\ell\over 2} < 1$.
    
    Chiamiamo $q = {1+\ell\over 2}$. Questo implica che ${a_{n+1}} < q \cdot a_n < 1$.
    
    Di conseguenza $\forall n > N \ a_{n+1} < q\cdot a_n < q^2 \cdot a_{n-1}<...< q^{(n+1)-N}a_N$, che implica $a_{n+1} < {a_N\over q^N} q^{n+1}$ $\Rightarrow$  $0< a_{n} < {a_N\over q^N} q^{n}$.
    
    Poiché $0< q< 1$  per costruzione, per il criterio del confronto la serie degli $a_n$ convergerà, convergendo quella di $q^n$.
    
2. Assumiamo ora che sia $\ell > 1$. 
    1. Se $\ell \in \R$, assumiamo $\epsilon = \frac{\ell-1}{2}$, da cui $\exist N \in \N :\forall n> N \, { a_{n+1}\over a_n} > \ell-\epsilon>1$. Questo significa che ${a_{n+1}\over a_n} > {1+\ell\over 2} > 1$.
        
        Chiamiamo $q = {1+\ell\over 2}$. Questo implica che ${a_{n+1}} > q \cdot a_n > 1$.
        
        Di conseguenza $\forall n > N \ a_{n+1} < q\cdot a_n < q^2 \cdot a_{n-1}<...< q^{(n+1)-N}a_N$, che implica $a_{n+1} > {a_N\over q^N} q^{n+1}$ $\Rightarrow$   $a_{n} > {a_N\over q^N} q^{n} >1$.
        
        Poiché $q>1$ per costruzione, per il criterio del confronto la serie degli $a_n$ divergerà, divergendo quella di $q^n$.
        
    2. Se $\ell = +\infty$, assumiamo $M = 2$ nella definizione di limite, da cui
    $\exist N \in \N : \forall n\ge N \ {a_{n+1}\over a_n} > M > 2$. Questo implica che $a_{n+1}> 2a_n$ e si ripete la dimostrazione fatta al punto precedente.

## 5.2 Criterio della radice *n-esima*

>Teorema: Criterio della radice N-esima
> **Sia $a_n$ una successione di termini definitivamente positivi in $n \in \N$ e $\exist \lim_{n\to\infty}\sqrt[n]{a_n}= \ell\in \overline \R$. Allora se**
> 
> 1. **$\ell > 1\Rightarrow \sum_{n=0}^{+\infty} a_n$  diverge e  $\lim_{n\to\infty}{a_n}= +\infty$**
> 2. **$0\le \ell < 1\Rightarrow \sum_{n=0}^{+\infty} a_n$  converge e  $\lim_{n\to\infty}{a_n}= 0$**

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Se $\ell = 1$  non è possibile concludere nulla sul carattere della serie, in quanto esistono serie che convergono e serie che divergono per quel valore di $\ell$. 


# 6. Altre serie per svolgere il confronto

Dai vari teoremi visti fin ora per le serie a termini definitivamente positivi è possibile trovare altre serie da aggiungere a quelle viste al paragrafo 3.2 di questo capitolo da poter utilizzare per svolgere il confronto.

- La serie $\sum_{n=1}^{+\infty} \frac{a^n}{n^n}$ **converge** $\forall a > 0$
- La serie $\sum_{n=1}^{+\infty} {a^n}{n^\alpha}, a > 0, \alpha \in \R$
    - **converge** per $0<a<1 \vee \forall\alpha\in \R$ e per $a = 1 \wedge \alpha < -1$
    - **diverge** per $a>1 \vee \forall\alpha\in \R$ e per $a = 1 \wedge \alpha \ge -1$.
- La serie $\sum_{n=1}^{+\infty} \frac{n!}{n^n}$ **converge**