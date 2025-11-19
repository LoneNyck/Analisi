# 18. Calcolo delle derivate e teoremi sulle derivate

Tags: Derivate, Dimostrazione importante
Data lezione: 14/11/2024

# 1. Derivate di funzioni elementari

Segue una tabella con le principali funzioni elementari e le loro derivate.

| ${f(x)}$ | ${f'(x)}$ |
| --- | --- |
| $c \in \R$ | 0 |
| $x^n$ | $n\cdot x^{n-1}, n\in \mathbb{N}$ |
| $x^\alpha$ | $\alpha \cdot x^{\alpha -1}, \alpha \in \R$ |
| $\sin x$ | $\cos x$ |
| $\cos x$ | $-\sin x$ |
| $e^x$ | $e^x$ |
| $\log x$ | $\frac1{x}$ |

## 1.1 Teorema di continuità delle funzioni derivabili
>Teorema
> **Se $f:(a,b) \to \R, x_0 \in (a,b)$ e $f$ derivabile in $x_0$, allora $f$ è continua in $x_0$.**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Il viceversa NON è vero, ossia esistono funzioni continue non derivabili. L’esempio più lampante è $f(x) = |x|$.


### 1.1.1 Dimostrazione

$f$ è derivabile per ipotesi, quindi $f$ è differenziabile per quanto visto in [17. Introduzione alle derivate](17%20Introduzione%20alle%20derivate%2013634a78851580e2b402f187f6457550.md), par. 5. 

$f(x)= f(x_0)+f'(x_0)(x-x_0)+o(x-x_0), x\to x_0$

$\Rightarrow$ $\lim_{x\to x_0}f(x)=\lim_{x\to x_0}f(x_0)+f'(x_0)(x-x_0)+o(x-x_0)= f(x_0)$.

Quindi $f(x)$ è continua in $x_0$.

# 2. Regole di derivazione

## 2.1 Derivate di somma, prodotto e quoziente di funzioni
> Teorema
> **Siano $f,g: (a,b)\to\R, x_0\in (a,b)$  e $f,g$ derivabili in $x_0$. Allora:**
> 
> - $\frac{d}{dx}[f(x_0)+g(x_0)] = f'(x_0) + g'(x_0)$;
> - **$\frac{d}{dx}[f(x_0)g(x_0)] = g(x_0)f'(x_0)+f(x_0)g'(x_0)$
> e in particolare $\forall \alpha \in \R$ $\frac{d}{dx}[\alpha f(x_0)]= \alpha f'(x_0)$;**
> - $\frac{d}{dx}[\frac{f(x_0)}{g(x_0)}] = \frac{g(x_0)f'(x_0)-f(x_0)g'(x_0)}{g^2(x_0)}$.

## 2.2 Derivata di composizione di funzioni
>Teorema
> **Sia $g\circ f(x) = g(f(x))$ composizione di due funzioni. Se $f$ è derivabile in $x_0$ e $g$ è derivabile in $t_0 = f(x_0)$ allora $g\circ f$  è derivabile in $x_0$ e vale $\frac{d}{dx}[g(f(x_0))]= g'(f(x_0))\cdot f'(x_0)$**
> 

## 2.3 Derivata dell’inversa di una funzione
>Teorema
> **Sia $f:(a,b)\to \R, x_0 \in (a,b), f \text { invertibile}, g = f^{-1}, f^{-1}(x_0) \ne 0, f \text{ continua in }(a,b)$. Allora $g$ è derivabile in $y_0= f(x_0)$ e $g'(y_0)= \frac 1{f'(x_0)}= \frac 1{f'(f^{-1}(y_0))}$.**
> 

# 3. Derivate e monotonia

>Definizione: Massimo locale 
**Sia $f:D_f\to \R, x_0 \in D_f$. Diremo che $x_0$ è punto di massimo locale se esiste un intorno $U(x_0)$ di $x_0$ $=(x_0 - \delta ; x_0 + \delta)$ tale che $f(x) \le f(x_0), \forall x\in U(x_0) \cap D_f$. Il corrispondente valore $f(x_0)$ si dice massimo locale.**

**Si dice inoltre che esso è stretto se $f(x) < f(x_0), \forall x\in U(x_0) \cap D_f$.**



>Definizione: Minimo locale
>**Sia $f:D_f\to \R, x_0 \in D_f$. Diremo che $x_0$ è punto di minimo locale se esiste un intorno $U(x_0)$ di $x_0$ $=(x_0 - \delta ; x_0 + \delta)$ tale che $f(x) \ge f(x_0), \forall x\in U(x_0) \cap D_f$. Il corrispondente valore $f(x_0)$ si dice minimo locale.**

**Si dice inoltre che esso è stretto se $f(x) > f(x_0), \forall x\in U(x_0) \cap D_f$.**

>Definizione: Massimo Globale
>**Sia $f:D_f\to \R, x_0 \in D_f$. Diremo che $x_0$ è punto di massimo globale se esiste un intorno $U(x_0)$ di $x_0$ $=(x_0 - \delta ; x_0 + \delta)$ tale che $f(x) \le f(x_0), \forall x\in  D_f$. Il corrispondente valore $f(x_0)$ si dice massimo globale.**

**Si dice inoltre che esso è stretto se $f(x) < f(x_0), \forall x\in  D_f$.**

>Definizione: Minimo globale
>**Sia $f:D_f\to \R, x_0 \in D_f$. Diremo che $x_0$ è punto di minimo globale se esiste un intorno $U(x_0)$ di $x_0$ $=(x_0 - \delta ; x_0 + \delta)$ tale che $f(x) \ge f(x_0), \forall x\in D_f$. Il corrispondente valore $f(x_0)$ si dice minimo globale.**

**Si dice inoltre che esso è stretto se $f(x) > f(x_0), \forall x\in D_f$.**

>Definizione: Estremo
>**Se $x_0$ è massimo oppure minimo per $f$, diremo che $x_0$ è punto di estremo o estremante per $f$.**


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
In un estremante $f$ può essere continua oppure no, può essere derivabile oppure no.


## 3.1 Teorema di Fermat
>Teorema di Fermat
> **Sia $f:(a,b)\to \R, x_0 \in (a,b)$. Se $x_0$ è punto di estremo per $f$ e se $f$ è  derivabile in $x_0$, allora $f'(x_0)=0.$**
> 

### 3.1.1 Dimostrazione

Dimostriamo il teorema nel caso in cui $x_0$  sia punto di **massimo** per la funzione.

Assumiamo $|h|$ sufficientemente piccolo - $|h|<\delta$  per il $\delta$  della definizione di massimo locale.
$\Rightarrow$  $f(x_0+h)\le f(x_0)$, in quanto $f(x_0)$  è massimo locale.

- $h>0$ $\Rightarrow$ $\frac{f(x_0+h)-f(x_0)}{h}\le 0$, essendo il numeratore negativo, mentre il denominatore positivo.
Essendo $f$ derivabile in $x_0$, per permanenza del segno segue che
$f'(x_0)=f_+'(x_0)=\lim_{h\to 0^+}\frac{f(x_0+h)-f(x_0)}{h}\le 0$
- $h<0$ $\Rightarrow$ $\frac{f(x_0+h)-f(x_0)}{h}\ge 0$, essendo sia numeratore che denominatore negativi.
Dato che $f$ è derivabile in $x_0$, per permanenza del segno segue che
$f'(x_0)=f_-'(x_0)=\lim_{h\to 0^-}\frac{f(x_0+h)-f(x_0)}{h}\ge 0$

$\Rightarrow$ $f'(x_0)\le 0 \wedge f'(x_0)\ge 0 \Leftrightarrow f'(x_0)=0$


>Definizione: Punto stazionario
**Se $f$ è derivabile in $x_0\in (a,b)$ e $f'(x_0)=0$, diremo che $x_0$ è punto stazionario o critico per $f$.**

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Esistono funzioni che hanno $f'(x_0) = 0$ in punti $x_0$ che non sono estremi per $f$. Un esempio può essere la funzione $f(x)=x^3$, che non presenta né massimi né minimi, ma ha derivata prima che si annulla in $x_0=0$.

Quindi $x_0 \max / \min \Rightarrow f'(x_0)=0$
$f'(x_0)=0 \nRightarrow x_0\max/\min$

![image.png](18%20Calcolo%20delle%20derivate%20e%20teoremi%20sulle%20derivate/image.png)

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" />**Osservazione**
Esistono punti stazionari che non sono né massimi, né minimi, né flessi.


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Possiamo combinare l’uso dei Teoremi di **Weierstrass** [[16. Proprietà globali di funzioni continue o monotone su un intervallo](16%20Propriet%C3%A0%20globali%20di%20funzioni%20continue%20o%20monoto%2013634a78851580e9939afa57df101e20.md), paragrafo 2] e di **Fermat** per **studiare** **massimi** e **minimi assoluti** di una funzione $f:(a,b)\to\R$ **continua**.

Per Weierstrass $f$ **ammette massimo e minimo** assoluti $\in [a,b]$. 

Per Fermat suddetti punti possono trovarsi solamente:

1. in un **punto stazionario**;
2. in un punto dove $f$ **non è derivabile**;
3. in uno dei due **estremi** $a,b$.

Tra questi punti, dove $f$ assume il valore più grande sarà il massimo assoluto, mentre dove assume il valore più piccolo sarà il minimo assoluto.


## 3.2 Teorema di Lagrange (o del valor medio)
>Teorema di Lagrange
> **Sia $f:[a,b]\to \R$ continua in $[a,b]$ e derivabile in $(a,b)$. Allora $\exists c \in (a,b)$ tale che $f'(c) = \frac{f(b)-f(a)}{b-a}$.**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione (Teorema di Rolle)**
Se si aggiunge alle ipotesi del teorema di Lagrange che $f(b) = f(a)$  la tesi diventa $\exists c \in (a,b) : f'(c) = 0$, che prende il nome di teorema di **Rolle**.


### 3.2.1 Dimostrazione

Introduciamo una funzione ausiliaria $g:(a,b)\to\R$, 
$g(x) = f(x)-[\frac{f(b)-f(a)}{b-a}(x-a)+f(a)]$, in cui la funzione tra parentesi corrisponde alla retta passante per i punti $(a;f(a))$ e $(b;f(b))$.
Allora:

1. $g$ è continua in quanto differenza di funzioni continue
2. $g$ è derivabile in quanto differenza di funzioni derivabili
3. $g(a)= 0$ e $g(b) =0$ $\Rightarrow g(a)=g(b)$

Da i. sappiamo che $g$ assume valore massimo $M$  e minimo $m$ per il Teorema di Weierstrass.

- Se $M= m$ , allora $g$ è costante e $g'(x)= 0, \forall x\in [a,b]$ 
$\Rightarrow 0 = g'(x)=f'(x)-\frac{f(b)-f(a)}{b-a}$ $\Rightarrow f'(x) = \frac{f(b)-f(a)}{b-a}, \forall x \in [a,b]$
- Se $M\ne m$, allora almeno uno dei due deve essere diverso da $0$ - che corrisponde alla quota di $a$ e $b$ - e quindi non può essere assunto negli estremi $a$ e $b$, ma in un punto $c\in (a,b)$
$\Rightarrow$  $c$ è punto di estremo $\Rightarrow$  $g'(c) =0$ per il Teorema di Fermat
$\Rightarrow$ $0 = g'(c)=f'(c)-\frac{f(b)-f(a)}{b-a}$ e per algebra dei limiti abbiamo che $f'(c) = \frac{f(b)-f(a)}{b-a}$

## 3.3 Teorema di caratterizzazione di funzioni costanti in un intervallo
>Teorema 
> **Sia $f:I\subseteq \R\to \R, I$  intervallo. Allora $f$ è costante in $I$ se e solo se $f$ è derivabile in $I$ e $f'(x) = 0,\forall x \in I$.**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Se $f:D_f \subseteq\R\to \R$ e $D_f\subseteq \R$ non è un intervallo, può accadere che 
$f'(x_0) = 0,\forall x \in D_f$   ma che $f$ non sia costante.


![image.png](18%20Calcolo%20delle%20derivate%20e%20teoremi%20sulle%20derivate/image%201.png)

### 3.3.1 Dimostrazione

1. Sia $f$ costante, quindi $f(x) = \lambda$, $\forall x \in I$
$f'(x_0) = \lim_{h\to 0}\frac{f(x_o+h)-f(x_0)}{h}= \lim_{h\to 0}\frac{\lambda-\lambda}{h} = 0$
Quindi $f$ è derivabile in $I$ e $f'(x) =0$
2. Siano $x_1,x_2 \in I$ . Sia $f'(x) =0$.
Assumiamo per semplicità che sia $x_1<x_2$ e consideriamo la funzione $g:[x_1;x_2]\to \R$, $g(x) = f(x)$. Allora $g$ è derivabile e quindi continua in $[x_1;x_2]$ essendolo $f$ per ipotesi.
    
    Per il Teorema di Lagrange $\exists c\in (x_1,x_2)\sub I$ tale che $g'(c) = \frac{g(x_2)-g(x_1)}{x_2-x_1}$
    $\Rightarrow$  $f'(c) = \frac{f(x_2)-f(x_1)}{x_2-x_1}=0$
    
    $\Rightarrow$ $f(x_2)-f(x_1)=0$ $\Rightarrow$ $f(x_2)=f(x_1), \forall x_1,x_2 \in I$
    $\Rightarrow f$ è costante.
    

## 3.4 Test di monotonia
>Test di monotonia
> **Sia $f:(a,b)\to \R$ derivabile in $(a,b)$. Allora:**
> 
> 1. **$f$ è crescente in $(a,b)$ $\Leftrightarrow$ $f'(x)\ge 0, \forall x\in (a,b)$**
> 2. **$f$ è decrescente in $(a,b)$ $\Leftrightarrow$ $f'(x)\le 0, \forall x\in (a,b)$**
> 3. **$f'(x)>0 , \forall x\in (a,b)\Rightarrow f$ è strettamente crescente**
> 4. **$f'(x)<0 , \forall x\in (a,b)\Rightarrow f$ è strettamente decrescente**

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Esistono funzioni strettamente crescenti e derivabili tali che $f'(x)\ge0,\forall x\in(a,b)$ ma che hanno $f'(x) = 0$ per qualche $x_0\in (a,b)$. Un esempio può essere la funzione $f(x) = x^3$.

Questo dipende dal fatto che nella dimostrazione viene utilizzato il teorema della permanenza del segno [[14. Teoremi sui limiti di funzioni](14%20Teoremi%20sui%20limiti%20di%20funzioni%2012f34a78851580fbbc8af41cb407c019.md), paragrafo 2] nella sua seconda forma.


![image.png](18%20Calcolo%20delle%20derivate%20e%20teoremi%20sulle%20derivate/image%202.png)

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**

L’ipotesi di definizione su un intervallo non può essere rimossa. Si pensi alla funzione $f(x) = \frac1x$, $f:(-\infty,0)\cup(0;+\infty)$, che ha derivata prima sempre minore di 0, ma non è decrescente su tutto il dominio, pur essendolo in ciascuno dei due intervalli singolarmente.


![image.png](18%20Calcolo%20delle%20derivate%20e%20teoremi%20sulle%20derivate/image%203.png)

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Il testo di monotonia permette di individuare massimi e minimi locali per $f$.


### 3.4.1 Dimostrazione

1. **$f$ è crescente in $(a,b)$ $\Leftrightarrow$ $f'(x)\ge 0, \forall x\in (a,b)$**
- Sia $f:(a,b)\to \R$ derivabile e crescente.
    
    Siano $x\in (a,b), h\in \R$ tale che $|h|$ sia abbastanza piccolo in modo che $x+h\in (a,b)$.
    Essendo $f$ crescente abbiamo che:
    
    - $h>0\Rightarrow x+h>x\Rightarrow f(x+h)>f(x)$
    - $h<0\Rightarrow x+h<x\Rightarrow f(x+h)<f(x)$
    
    Per $h\ne 0$ vale in ambedue i casi che $\frac{f(x+h)-f(x)}{h}\ge 0$
    Poiché $f$ è derivabile, per permanenza del segno vale che
    $f'(x)=\lim_{h\to0}\frac{f(x+h)-f(x)}{h}\ge 0$
    $\Rightarrow f'(x)\ge 0, \forall x\in (a,b)$
    
- Sia $f:(a,b)\to \R$ derivabile e $f'(x)\ge 0, \forall x\in (a,b)$.
    
    Siano $x_1,x_2\in (a,b)$ e assumiamo sia $x_1<x_2$, per comodità. 
    $[x_1;x_2]\sub(a,b)$ e poiché $f$ è derivabile in $(a;b)$ essa lo sarà anche in $(x_1;x_2)$, e quindi sarà anche continua in $[x_1;x_2]$.
    Per il Teorema di Lagrange applicato alla restrizione di $f$, esiste un punto $c\in (x_1,x_2)$ tale che $f'(c) = \frac{f(x_2)-f(x_1)}{x_2-x_1}\ge 0$, in quanto $f'(x)\ge 0, \forall x\in (a,b)$ per ipotesi.
    
    Essendo $x_2 > x_1$ deve valere necessariamente che $f(x_2)\ge f(x_1)$.
    $\Rightarrow$  $f(x_2)\ge f(x_1)\Rightarrow f$ è crescente.
    

iii**. $f'(x)>0 , \forall x\in (a,b)\Rightarrow f$ è strettamente crescente**
La dimostrazione di questo punto è identica a quella appena svolta, l’unica differenza è che le disuguaglianze sono strette.

Siano $x_1,x_2\in (a,b)$ e assumiamo sia $x_1<x_2$. 
$[x_1;x_2]\sub(a,b)$ e poiché $f$ è derivabile in $(a;b)$ essa lo sarà anche in $(x_1;x_2)$, e quindi sarà anche continua in $[x_1;x_2]$.
Per il Teorema di Lagrange applicato alla restrizione di $f$, esiste un punto $c\in (x_1;x_2)$ tale che $f'(c) = \frac{f(x_2)-f(x_1)}{x_2-x_1}> 0$, in quanto $f'(x)> 0, \forall x\in (a,b)$ per ipotesi.

Essendo $x_2 > x_1$ deve valere necessariamente che $f(x_2)> f(x_1)$.
$\Rightarrow$  $f(x_2)> f(x_1)\Rightarrow f$ è strettamente crescente.


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**

Se $f(a,b)\to \R$ è derivabile, allora $f'(x_0)> 0\in (a,b)$ $\Rightarrow f$ è strettamente crescente in $(a,b)$ $\Rightarrow f$ è invertibile in $(a,b)$


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" />**Osservazione** sul rapporto tra funzioni e successioni

Per dimostrare che una successione $a_n$ sia monotona serve dimostrare che $a_n \ge a_{n+1}, \forall n\in \mathbb{N}$ (o $a_n \ge a_{n+1}, \forall n\in \mathbb{N}$).

Tuttavia se si riesce a definire una funzione $f(n):[0,+\infty)\to \R$ monotona crescente (o decrescente) tale che $f(n) = A_n ,\forall n \in \mathbb{N}$, allora si può dedurre che $a_n$ha la stessa monotonia della funzione.

$a_n = f(n) \le f(n+1)= a_{n+1}$ se $f$ cresce
$a_n = f(n) \ge f(n+1)= a_{n+1}$  se $f$ decresce

Per dimostrare la monotonia di $f$ è sufficiente mostrare che $f$ sia derivabile e $f'(x)\ge0$ (o $f'(x)\le0), \forall x\in [0,+\infty)$ in virtù del test di monotonia.

Può accadere che $a_n$ sia monotona e che una sua interpolazione $f$ non lo sia, questo perché la condizione è sufficiente, ma non necessaria.


# 4. Teorema di De L’Hôpital
>Teorema di De L’Hôpital
> **Siano $f,g:(a,b)\to\R$ derivabili, $g,g'\ne0\in (a,b)$. Se accade che**
> 
> 1. **$\lim _{x\to a^+}f(x)=\lim _{x\to a^+}g(x)=0$  oppure $\lim _{x\to a^+}f(x)=\pm \infty$ e $\lim _{x\to a^+}g(x)=\pm\infty$  (non necessariamente concordi in segno)**
> 2. $\exists \lim _{x\to a^+}\frac{f'(x)}{g'(x)}=\ell\in \overline \R$
> 
> **allora $\exists \lim _{x\to a^+}\frac{f(x)}{g(x)}=\ell\in \overline \R$.**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" />**Osservazioni**

- Il teorema vale anche nel caso in cui $a= -\infty$
- Il teorema vale anche nei casi $\lim_{x\to b^-}...$ e $\lim_{x\to x_0}...$
- Il teorema copre solo il caso di indeterminazione $\frac 00$ oppure $\frac \infty \infty$

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**

**Se $\nexists \lim _{x\to a^+}\frac{f'(x)}{g'(x)}$, non si può concludere nulla su $\lim _{x\to a^+}\frac{f(x)}{g(x)}$.**


Mediante il Teorema di de L’Hôpital è possibile dimostrare la gerarchia degli inifiniti, essendo i suoi casi nella forma di indeterminazione $\frac \infty \infty$. 

# 5. Teorema del prolungamento della derivata prima
>Teorema
> **Sia $f:[a,b)\to\R$ continua in $[a,b)$ e derivabile in $(a,b)$. Supponiamo che $\lim_{x\to a^+}f'(x)= m \in \overline \R$. 
Allora $\exists f_+'(a)=\lim_{h\to 0^+}\frac{f(a+h)-f(a)}{h}=m\in \overline \R$**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" />**Osservazione**
Sotto le ipotesi del teorema opportunamene modificate, vale il medesimo risultato anche per derivata sinistra $f_-'(b)$ e per la derivata $f'(x_0)$. La tesi diviene allora:
$\exists f_-'(b)=\lim_{x\to b^+}f'(x)= m \in \overline \R$ nel primo caso;
$\exists f'(x_0)=\lim_{x\to x_0}f'(x)= m \in \overline \R$ nel secondo caso.


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazioni**

- È possibile che $\nexists \lim_{x\to a^+}f'(x)$, ma esista $f_+'(a)$. Un caso può essere la funzione $f(x) = x^2\sin \frac 1x, x\ne 0$, con $f(0) = 0$.
- Non è possibile rimuovere dal teorema l’ipotesi di continuità della funzione. In tal caso potrebbe esistere il limite della derivata nel punto di discontinuità, ma non esisterebbe la derivata, non essendo la funzione ivi derivabile.

![image.png](18%20Calcolo%20delle%20derivate%20e%20teoremi%20sulle%20derivate/image%204.png)

## 5.1 Dimostrazione

Sia $h> 0$ in modo che $a+h \in (a,b)$. Applichiamo il teorema di Lagrange in $[a,a+h]$. Poiché $[a,a+h]\sub[a,b)$ e $(a,a+h)\sub (a,b)$, $f$ sarà continua e derivabile rispettivamente nel primo e nel secondo intervallo. 

Per Lagrange $\exists c_h\in [a,a+h]:f'(c_h)= \frac{f(a+h)-f(a)}{h}$. Per costruzione vale che 
$a\le c_h\le a+h$, quindi per $h\to 0, c_h\to a^+$ per il teorema del confronto.

$\lim_{h\to0^+}\frac{f(a+h)-f(a)}{h}=\lim_{h\to0^+}f'(c_h)=\lim_{t\to a^+}f'(t)$, con il cambio di variabile $t= c_h$, in quanto $h\to0^+,  c_h\to a^+$. Sia $\lim_{t\to a^+}f'(t)=m$.

Allora $\exists f'_+(a)=\lim_{h\to0^+}\frac{f(a+h)-f(a)}{h}=m\in \overline \R$.

## 5.2 Corollario
>Corollario
> **Sia $f:I\subseteq\R\to\R$ con $I$  intervallo. Supponiamo $\exists f':I\to\R$, ossia $f$ sia derivabile $\forall x \in I$. Allora $f'$ può avere in $I$ solo punti di discontinuità di II specie**
> 

La derivata prima non può quindi presentare discontinuità eliminabili o discontinuità a salto e la funzione non può pertanto avere punti angolosi.

### 5.2.1 Dimostrazione

Per il Teorema di prolungamento della derivata $f_+'(x_0)=\lim_{x\to x_0^+}f'(x)$ e 

$f_-'(x_0)=\lim_{x\to x_0^-}f'(x)$ se tali limiti esistono. Poiché $f'(x_0)\in \R$ per ipotesi, se tali limiti esistono, allora essi sono costretti a coincidere con $f'(x_0)$. In particolare $x_0$ non può essere punto di discontinuità eliminabile né a salto.

# 6. Teorema di Darboux
>Teorema
> **Sia $f:I\subseteq\R\to\R$ con $I$  intervallo. Supponiamo $\exists f':I\to\R$. Allora per ogni coppia di punti $a,b\in I$  con $a<b$, la funzione $f'$ assume tutti i valori compresi tra $f'(a)$  e $f'(b)$ in $(a,b)\subseteq I$**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Questo teorema è valido sia nel caso in cui $f'$ sia continua, che in quello in cui non lo sia.
