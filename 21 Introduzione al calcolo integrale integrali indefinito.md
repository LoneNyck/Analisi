# 21. Introduzione al calcolo integrale: integrali indefiniti

Tags: Integrali
Data lezione: 28/11/2024

# 1. Primitiva della funzione

>Definizione: Primitiva
>**Data $f:I\subseteq\R\to\R$ e $F:I\to\R$ diremo che $F$ è primitiva di $f$ in $I$ se**
>1. **$F$ è derivabile in $I$**
>2. **$F'(x) = f(x),\forall x\in \R$**

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Data $f:I\subseteq\R\to\R$, $I$ intervallo, non è detto che essa ammetta primitiva in $I$.

Un’esempio può essere la la funzione che vale 0 in $[-1,0)$ e 1 in $[0,1]$, oppure la funzione segno, le quali non ammettono primitiva perché hanno punti di discontinuità di tipo salto in $x_0$ e non soddisfano la proprietà dei valori intermedi (in particolare il teorema di Darboux). Per i teoremi visti sui punti di discontinuità delle funzioni definite e derivabili, $f$ non può essere derivata di alcuna funzione nell’intervallo $[-1,1]$


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Data $f:I\subseteq\R\to\R$, $I$ intervallo, e $f$ continua in $I$, allora essa ammette primitiva. Questo prenderà il nome di Teorema fondamentale del calcolo integrale, che vedremo in seguito.


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Esistono funzioni non continue che ammettono comunque primitiva.

>Teorema
> **Se $F:I\subseteq\R\to\R$ è una primitiva di $f:I\subseteq \R\to\R$ in $I$ e $c\in \R$, allora anche $F(x)+c$ è una primitiva di $f$ in $I.$
Analogamente se sono date due primitive $F_1,F_2$ di $f$ sempre dal medesimo intervallo a $\R$, allora
$\exists c\in \R:F_1(x)=F_2(x)-c, \forall x \in \R$**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Da quanto appena enunciato possiamo concludere che $f$  può non ammettere primitiva, ma se essa esiste, allora ve ne sono infinite, tutte e sole nella forma $F(x)+c$ per $c$ arbitrario.


## 1.1 Dimostrazione

1. Deriviamo $F+c$ rispetto ad x.
    
    $$
    \frac{d}{dx}[F(x)+c]=F'(x)+0=f(x)
    $$
    
    Per definizione di primitiva, $F+c$ è primitiva di $f$ in $I$
    
2. Siano $F_1 , F_2$ due primitive di $f$. Sia $G(x) = F_1(x)-F_2(x)$. $G$ è derivabile in quanto somma di funzioni derivabili e vale che $G'(x) = F'_1(x) -F'_2(x) = f(x) -f(x) = 0$. Per il teorema della caratterizzazione di funzioni costanti vale che $G$ è costante in $I$ e di conseguenza $F_1(x)-F_2(x) = c$. 

# 2. Integrali notevoli e integrale indefinito

Segue una tabella con i principali integrali notevoli, ricavati mediante l’inversione delle derivate.

| $f(x)$ | $F(x)$ |
| --- | --- |
| $k$ | $kx+c$ |
| $x^n$ | $\frac{x^{n+1}}{n+1}+c$ |
| $x^\alpha$ | $\frac{x^{\alpha+1}}{\alpha+1}+c$ |
| $\frac 1x$ | $\log\|x\|+c$ |
| $\cos x$ | $\sin x+c$ |
| $\sin x$ | $-\cos x+c$ |
| $e^{\alpha x}$ | $\frac{e^{\alpha x}}{\alpha}+c$ |
| $\frac{1}{1+x^2}$ | $\arctan x+c$ |
| $\frac{1} {\sqrt{1+x^2}}$ | $\arcsin x +c$ |
| $\cosh x$ | $\sinh x+c$ |


>Definizione: Integrale indefinito
>**L’insieme di tutte le primitive di $f:I\subseteq\R\to\R$ prende il nome di integrale indefinito di $f$ e si indica con**
>$$
\int f(x)\ dx
$$


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Se $F(x)$ è primitiva, spesso si scrive

$$
\int f(x) \ dx = F(x) +c
$$


# 3. Regole di integrazione

## 3.1 Linearità dell’integrale

>Teorema
> **Siano $f,g:I\subseteq\R\to\R, \alpha,\beta\in \R$. Allora**
> $$
>   \int \alpha f(x)+\beta g(x) \ dx = \alpha \int f(x) \ dx + \beta \int g(x) \ dx
> $$
>

## 3.2 Integrazione per parti
>Teorema
> **Siano $f,g:I\subseteq\R\to\R, I$  intervallo,  funzioni derivabili in $I$. Allora**
> 
> $$
>  \int f'(x)g(x) \ dx = f(x)g(x)-\int f(x)g'(x) \ dx
> $$
> 

## 3.3 Integrale per sostituzione / integrazione di funzioni composte

> **Siano $f:I\subseteq\R\to\R, I$  intervallo,  e $\psi :J\to I , J$  intervallo, $\psi$  derivabile in $J$. Allora**
> 
> 
> $$
>  \int \psi'(t)f(\psi(t)) \ dt = \int f(x) \ dx , \text{con } x = \psi (t)
> $$
> 


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**

Esiste un algoritmo per calcolare $\int \frac {P(x)}{Q(x)}\ dx$ , dove $P(x), Q(x)$ sono polinomi di grado qualsiasi, chiamato [Scomposizione in fratti semplici](21%20Introduzione%20al%20calcolo%20integrale%20integrali%20ind/Scomposizione%20in%20fratti%20semplici%2014c34a78851580dabd8ae66a5ec23c6c.md).
