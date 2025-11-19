# 5. Numeri complessi

Tags: Numeri complessi
Data lezione: 25/09/2024

# 1. Unità immaginaria

$x^2 +1 = 0$ non ha soluzione in $\R$ o in alcun campo ordinato, in quanto:
$x^2 \ge 0, \forall x \in X$
$1>0$
$\Rightarrow x^2 +1 \ge 1 > 0 \Rightarrow x^2 +1 \neq 0$

È possibile estendere $\R$ per far sì che l’equazione ammetta soluzione?

> Definizione: Unità immaginaria
>**L’unità immaginaria $i$ è definita come $i^2 +1 = 0$**


# 2. Insieme dei numeri complessi e forma algebrica

> Definizione: Insieme dei numeri complessi
>**Definiamo $\mathbb{C} = \{ z = a+bi: a, b \in \R, i^2+1 = 0\}$** 

>Definizione: forma algebrica
>**$z = a+bi$ prende il nome di forma algebrica del numero complesso $z$.**


$a$ prende il nome di **parte reale** del numero complesso e viene indicata come $\Re{z}$; $b$  prende invece il nome di **parte immaginaria** del numero complesso e viene indicata come $\Im z$

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px"/> **Osservazione**
$\Re z , \Im z \in \R, \forall z \in \mathbb{C}$


# 3. Operazioni in $\mathbb{C}$

In $\mathbb{C}$ sono definite le operazioni di **somma** e **prodotto** (e le relative inverse, rispettivamente differenza e divisione), entrambe dotate delle proprietà già viste in [1. Introduzione: insiemi numerici, logica e quantificatori](1%20Introduzione%20insiemi%20numerici,%20logica%20e%20quantifi%208086083780cf49709b466f3c30350a75.md), paragrafo 2. 

Dati due numeri complessi $z$   e $w$, $\forall z = a+bi$  e $\forall w = x + yi$  $\in \mathbb{C}$, la **somma** tra i due è così definita:
$z+w = (a+x) +(b+y)i$

Dati gli stessi numeri complessi, il **prodotto** tra di essi è così definito:
$z\cdot w = (ax-by) +(bx+ay)i$


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px"/> **Osservazione**
Le operazioni di $+$ e $\cdot$ vengono formalmente definite come somma e prodotto di polinomi a coefficienti reali in $i$ : $i^2  =-1$

Ne consegue quindi che, come già accennato in [3. Campi, insiemistica e intervalli](3%20Campi,%20insiemistica%20e%20intervalli%20eb86f163c8994969a366838e8e38ffc6.md), paragrafo 1:

> Teorema
> **$\mathbb{C}$ è un campo.**

## 3.1 Elementi neutri, opposto e inverso

Dato il numero complesso $z = a+bi$ si definiscono:

- **Elemento neutro** per la somma:
$0 = 0+0i$
- **Elemento neutro** per il prodotto:
$1 = 1 +0i$
- **Elemento opposto:**
$-z = -a -bi$
- **Elemento inverso**:
$z^{-1}= {1 \over z} = {a \over a^ 2 + b^2} -{b \over a^ 2 + b^2}i$


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
$\R$ è un **sottocampo** di $\mathbb{C}$.

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
$\R$ può essere identificato con i punti di una retta, $\mathbb{C}$ con quelli di un **piano** - che prende il nome di piano di Gauss.  $z = a+bi$ corrisponde pertanto al punto $Z$ di coordinate $(a,b) \in \R^2$. In particolare, inoltre, ogni numero complesso può essere pensato come un vettore nel piano applicato in $O$ e avente l’altro estremo in $Z$, orientato da $O$ a $Z.$


La somma tra due numeri complessi a livello geometrico corrisponde quindi alla somma di due vettori, corrispondente quindi ad una traslazione.

# 4. Coniugato e modulo

>Definizione: complesso coniugato e modulo
>**Dato un numero complesso $z = a +bi$, chiamiamo $\overline{z} = a-bi$ il complesso coniugato di $z \in \mathbb{C}$.  Indichiamo con $|{z}| = \sqrt{a^2 + b^2}$  il modulo di $z \in \mathbb{C}$.**


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazioni**
- $|z| = 0 \Leftrightarrow a = 0 \wedge b = 0 \Leftrightarrow  z= 0$
- $| z| \ge 0 , \forall z \in \mathbb{C}$
- $z = \overline z \Leftrightarrow z \in \R$


$\overline z$  è il **simmetrico** di $z \in \mathbb{C}$ rispetto all’asse reale $\forall z \in \mathbb{C}$; $|z|$ è la distanza di $z \in \mathbb{C}$ da $O$ nel piano complesso, $\forall z \in \mathbb{C}$. $|z-w|$  è la **distanza** di $z \in \mathbb{C}$ da $w \in \mathbb{C}$ nel piano complesso.

Nel piano complesso: 

- $\Im z$ costante corrisponde ad una **retta orizzontale** nel piano complesso;
- $\Re z$ costante corrisponde ad una **retta verticale** nel piano complesso;
- $|z|$  costante corrisponde ad una **circonferenza** centrata nell’origine con raggio $|z|$ stesso.

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazioni**
- $z \overline z = (x+iy)(x-iy) = x^2 +y^2  = |z|^2 ,\forall z = x+iy \in \mathbb{C}$
- $|z| = | \overline z |, \forall z \in \mathbb{C}$
- $z^{-1} = {1 \over z} \cdot { \overline z \over \overline z} ={\overline z \over |z| ^2}, \forall z \in \mathbb{C}, z \neq 0$
- $\overline {w+z} = \overline z + \overline w, \forall w,z \in \mathbb{C}$
- $\overline {wz} = \overline w \cdot \overline z, \forall w,z \in \mathbb{C}$
- ${z \over w } = {z \overline w\over |w|^2}, \forall w,z \in \mathbb{C}, w \neq 0$

# 5. Forma trigonometrica e forma esponenziale

Alternativamente alla forma algebrica di $z$  - in cui assegniamo $x = \Re z$, $y = \Im z$, da cui 
$z = x +iy \in \mathbb{C}$, possiamo individuare il numero complesso assegnando $\rho = \sqrt{x^2 + y^2}$ e $\theta = \arg z$, che corrisponde all’angolo orientato formato dal semiasse delle ascisse positive e dalla semiretta uscente da $O$ e passante per $z$ - angolo positivo se in senso antiorario, negativo altrimenti.

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazioni**
- $\arg 0$ non è ben definito.
- L’argomento di un numero complesso $z\neq0$ è definito a meno di multipli interi di $2\pi$, ossia se $\arg z = \theta = \theta + 2k\pi , \forall k \in \mathbb{Z}$

Nel piano complesso $\theta$  costante corrisponde ad una **semiretta** uscente da $O$, esclusa l’origine degli assi. 

$\biggl\{\begin{aligned} &x = \Re z= \rho \cos\theta \\  &y = \Im z= \rho \sin\theta \end{aligned}$

Possiamo quindi concludere che:

$$
\begin{cases} \cos\theta = {x \over \rho} = {x \over \sqrt{x^2 + y^2}}  \\  \sin\theta = {y \over \rho} = {y \over \sqrt{x^2 + y^2}} \end{cases} \Rightarrow \tan\theta = {y \over x }
$$

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
In generale può NON essere vero che $\theta = \arccos {x \over \rho}$, $\theta = \arcsin {y \over \rho}$ e $\theta = \arctan {y \over x}$

> Definizione: Argomento pricipale 
> **Si chiama argomento principale di $z \in \mathbb{C}$ l’unico argomento di $z$ in $[0,2\pi)$ o in $[-\pi,\pi]$.**

> Definizione: Forma trigonometrica
> **Dato il numero complesso $z \in \mathbb{C}, z= x+yi$, $z = \rho (\cos\theta +i\sin\theta)$ prende il nome di rappresentazione in forma trigonometrica del numero complesso.**

>Definizione: forma esponenziale
>**Dato il numero complesso $z \in \mathbb{C}, z= x+yi = \rho (\cos\theta +i\sin\theta)$, $z = \rho e ^{i \theta}$ prende il nome di rappresentazione in forma esponenziale del numero complesso.**


## **5.1 Formula di Eulero**

La **formula di Eulero** afferma che $e^{i \theta} = \cos\theta + i \sin\theta$. Dimostreremo in seguito il perché di questa formula [[20. Approssimazioni polinomiali e polinomi di Taylor](20%20Approssimazioni%20polinomiali%20e%20polinomi%20di%20Taylo%2014634a78851580d4a9a7dbb3ed696623.md) ]

# 6. Formule di De Moivre

Seguono le Formule di De Moivre per il calcolo di numeri prodotti e rapporti tra numeri complessi.
> Teorema
> **Dati $w = \sigma(\cos\phi + i \sin\phi) = \sigma e^{i\phi} \in \mathbb{C}$ e 
$z = \rho (\cos\theta +i\sin\theta) = \rho e^{i \theta}$ 
$\Rightarrow$ $z\cdot w = \rho\sigma(\cos(\theta + \phi) + i \sin(\theta + \phi)) = \rho \sigma e^{i (\theta + \phi)}$**
> 
> **Inoltre se $w \neq 0$
> $\Rightarrow$  ${z\over w} = {\rho \over \sigma}(\cos(\theta - \phi) + i \sin(\theta - \phi)) = {\rho \over \sigma} e^{i (\theta - \phi)}$**


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazioni**

- $|z\cdot w| = |z| \cdot |w|$
- $|{z\over w}| = {|z| \over |w|}$
- $\arg (z\cdot w) = \arg z +\arg w$
- $\arg ({z\over w}) = {\arg z - \arg w}$

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Se $z = 1$ $\Rightarrow$  ${1\over \sigma}(\cos(\phi) - i \sin(\phi)) = {1\over \sigma} e^{i (-\phi)}$

Dalla formula di De Moivre per il prodotto è possibile ricavare la formula per la potenza di un numero complesso $z$.

>Teorema 
> **Dati $z \in \mathbb{C}$, $n \in \mathbb{N}$, $z^n = \rho^n (\cos n\theta +i\sin n\theta) = \rho^n e ^{i n\theta}$**
> 
> **Inoltre se $z\neq 0$, $z^{-n} = {1 \over z^n} (\cos n\theta -i\sin n\theta) =  {1 \over z^n}e ^{-in\theta}$**
> 

Tutte le precedenti sono formule **coerenti** con l’algebra degli esponenziali.

# 7. Radici *n-esime* del numero complesso

>Definizione: radice n-esima del numero complesso
>**Se $w \in \mathbb{C}$, $n \in \mathbb{N}, n\ge 1$ $\Rightarrow$  ogni numero complesso $z \in \mathbb{C}$ tale che $z^n = w$ prende il nome di radice *n-esima* di $w$.**

> Teroema
> **Si dimostra che esistono esattamente  $n$ radici complesse *n-esime* di $w$.**

Se $w = \rho e^{i\theta} = \rho (\cos \theta + i \sin \theta)$, allora le radice complesse *n-esime* $z_0,z_1, z_2,...,z_n$ hanno la forma:
$z_k = \rho ^ {1 \over n}(cos\phi_k + i \sin \phi_k) = \rho^ {1 \over n} e^{i\phi_k}$ con $\phi_k = {1 \over n}(\theta + 2k\pi)  = { \theta + 2k\pi \over n}$, per 
$k = 0,1,...,n-1$

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Tutte le radici n-esime di $w \in \mathbb{C}$ hanno il **medesimo modulo**, ossia nel piano complesso giacciono sulla medesima circonferenza di centro $O$ e di raggio $|w|^{1\over n}$. Inoltre radici successive hanno argomenti che differiscono di $2 \pi \over n$, **angolo fisso** - cioè l’angolo al centro è lo stesso per ogni coppia di radici successive. 


Ne consegue che $n$ radici complesse si dispongono a formare un **poligono regolare** di altrettanti lati, inscritto nella circonferenza di centro $O$  e raggio $|w|^{1\over n}$.

Le radici *n-esime* di un numero complesso $w \in \mathbb{C}, w \neq 0$ formano un **insieme** di $n$  numeri complessi.

La radice *n-esima* di un numero complesso **NON è una funzione** da $\mathbb{C} \to \mathbb{C}$, associando ad un numero più di una soluzione. 

![image.png](5%20Numeri%20complessi/image.png)

![image.png](5%20Numeri%20complessi/image%201.png)

# 8. Equazioni di secondo grado in $\mathbb{C}$

Date $a,b,c, \in \mathbb{C}, a\neq0$ $\Rightarrow$  $az^2+bz+c = 0$ ha necessariamente due soluzioni per quanto detto nel paragrafo precedente.

Per risolvere tale equazione è possibile **sostituire** $z = x +iy$ e risolvere un sistema a due equazioni e due variabili in $\R$; alternativamente possiamo porre $\Delta = b^2 -4ac$, da cui
$z_1,z_2 = {-b + \sqrt{\Delta}\over 2a}$, con $\Delta \in \mathbb{C}$.

In particolare vale la **formula di fattorizzazione** delle radici di un’equazione, per la quale
$\forall z \in \mathbb{C}, az^2+bz+c = a(z-z_1)(z-z_2)$

# 9. Teorema fondamentale dell’algebra

>Teorema fondamentale dell'alegbra
> **Un’equazione polinomiale della forma 
$a_nz^n+a_{n-1}z^{n-1}+...+a_1z+a_0 = 0$, con 
$a_n, a_{n-1},...,a_1, a_0 \in \mathbb{C}, a_n \neq 0, n\in \mathbb{N}, n\ge1$  ha esattamente $n$ soluzioni in $\mathbb{C}$ se ciascuna di esse è contata con le dovute molteplicità - ossia le radici possono essere non tutte distinte.**
> 

Dette $z_0, z_1,...,z_{n-1} \in \mathbb{C}$ tali soluzioni, allora $\forall z \in \mathbb{C}$ vale
$a_nz^n+a_{n-1}z^{n-1}+...+a_1z+a_0 = a_n(z-z_0)(z-z_1)...(z-z_{n-1})$

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
$z - \overline z = 0$ non è un’equazione polinomiale in $\mathbb{C}$ in quanto $z - \overline z$ non è un polinomio in $z$. 