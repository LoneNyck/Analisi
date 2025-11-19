# 17. Introduzione alle derivate

Tags: Derivate, Dimostrazione importante
Data lezione: 07/11/2024

# 1. Rapporto incrementale

Sia $f: (a,b) \to \R, x_0\in (a,b).$ Sia $h \in \R$, con $|h|$ sufficientemente piccolo, in modo che $x_0 +h \in (a,b)$. Consideriamo i punti $P_0(x_0, f(x_0)$ e $P_h(x_0+h, f(x_0+h))$, $h\ne 0$. Allora $\Delta x  = h$  e $\Delta y = f(x_0+h)-f(x_0)$.
La retta passante per i punti $P_0$ e $P_h$ avrà **coefficiente angolare** $m_h = \frac{\Delta y}{\Delta x}=\frac{f(x_0+h)-f(x_0)}{h}$, che corrisponde alla “pendenza media” del grafico di $f$ in $(x_0, x_0 +h)$. Contestualmente $m_h$ varia e può accadere che al tendere di $h \to 0$, esso tenda ad un valore finito. In tal caso la retta si stabilizza su una posizione per $h\to0$. Vogliamo definire tale retta come la **retta tangente** al grafico di $f$ nel punto $P_0$.

>Definizione: Rapporto incrementale
>**Sia $f: (a,b) \to \R, x_0 \in (a,b), h \in \R\setminus \{0\}$  e $x_0+h \in (a,b)$. Allora $\frac{f(x_0+h)-f(x_0)}{h}$ viene chiamato rapporto incrementale di $f$ in $x_0$, con incremento $h$.**


# 2. Derivata prima, retta tangente e derivata destra e sinistra

>Definizione: Derivabile
**Sia $f: (a,b) \to \R, x_0 \in (a,b)$. Diremo che $f$ è derivabile in $x_0$ se esiste finito  $\lim_{h\to 0}\frac{f(x_0+h)-f(x_0)}{h}\in \R$. Tale limite prende il nome di derivata prima di $f$ in  $x_0$ e scriveremo $f'(x_0) = \lim_{h\to 0}\frac{f(x_0+h)-f(x_0)}{h}$.
Altri modi di indicare la derivata sono i seguenti: $\frac{df}{dx}(x_0), Df(x_0), \dot f(x_0)$.**

>Definizione: Tangenza
**Se $f: (a,b) \to \R, x_0 \in (a,b)$ è derivabile in $x_0$, si definisce retta tangente al grafico di $f$ in $P_0(x_0, f(x_0))$ la retta $y = f'(x_0) (x-x_0)+f(x_0)$**

>Definizione: Derivate destra e sinistra
>**Definiamo derivata destra di $f$  in $x_0$ $f_+'(x_0) = \lim_{h\to 0^+}\frac{f(x_0+h)-f(x_0)}{h}$.**
>
>**Definiamo derivata sinistra di $f$  in $x_0$ $f_-'(x_0) = \lim_{h\to 0^-}\frac{f(x_0+h)-f(x_0)}{h}$.**


Si noti che **se derivata destra e derivata sinistra** nel punto $x_0$ **non coincidono,** allora la **funzione non è derivabile** in quel punto e ivi non ammette tangente.

Si noti che se $f:(a,b)\to\R$ è derivabile $\forall x_0\in (a,b)$, risulta allora definita la **funzione** **derivata** **prima** **di** $f$ $f': (a,b) \to \R$.

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
$f'(x_0) = \lim_{h\to 0}\frac{f(x_0+h)-f(x_0)}{h}=\lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0}$, sostituendo $x_0 + h = x$, da cui $h = x-x_0$. Per $h\to 0$, $x \to x_0$.


# 3. Derivate di gradi superiore al primo e derivata non finita

>Definizone: derivata seconda
**Se $f: (a,b) \to \R, x_0 \in (a,b)$ è derivabile in un intorno $U(x_0)$  di $x_0$, incluso $x_0$, e se esiste finito $\lim_{h\to 0}\frac{f'(x_0+h)-f'(x_0)}{h}\in \R$, chiameremo tale limite derivata seconda di $f$ in $x_0$ e scriveremo $f''(x)=\lim_{h\to 0}\frac{f'(x_0+h)-f'(x_0)}{h}\in \R$**

>Definizione: Derivata n-esima
>**Se $f: (a,b) \to \R, x_0 \in (a,b)$ è derivabile $(n-1)$ volte in un intorno $U(x_0)$  di $x_0$ (incluso $x_0$), con $n\ge 2$,  e se esiste finito $\lim_{h\to 0}\frac{f^{(n-1)}(x_0+h)-f^{(n-1)}(x_0)}{h}\in \R$, diremo che $f$ è derivabile $n$ volte in $x_0$ e chiameremo tale limite derivata n-esima di $f$ in $x_0$  e scriveremo $f^{n}(x_0)=\lim_{h\to 0}\frac{f^{(n-1)}(x_0+h)-f^{(n-1)}(x_0)}{h}\in \R$.**


Se $f:(a,b)\to \R, x_0 \in (a,b)$ e $f$ continua in $x_0$ ed esiste il limite del rapporto incrementale in $x_0$ infinito diremo che $f$ **non è derivabile** in $x_0$, ma scriveremo $f'(x_0)=\pm \infty$ con abuso di notazione. In tal caso la retta tangente al grafico in $P(x_0,f(x_0))$ è la retta verticale $x= x_0$.

# 4. Variazione istantanea

Siano $f:(a,b)\to \R, x_0 \in (a,b)$ e $h> 0$ abbastanza piccolo in modo che $x_0+h\in (a,b)$. L’espressione $\frac{f(x_0+h)-f(x_0)}{h}= \frac{\Delta f}{\Delta x}$ esprime la **variazione media** di $y = f(x)$ nell’intervallo $x_0, x_0+h$. Se f è derivabile in $x_0$, $f'(x_0) = \lim_{h\to 0}\frac{f(x_o+h)-f(x_0)}{h} \in \R$ esprime il tasso di **variazione istantanea** di $y = f(x)$ al variare di $x$ , in $x= x_0$. 

In particolare se $y=s(t)$  è una legge oraria, $s'(t)$ è la velocità istantanea; se $y=v(t)$ è la velocità, $v'(t)$ è l’accelerazione istantanea; se $y = \theta (t)$ è l’angolo di rotazione, $\theta'(t)$  è la velocità angolare istantanea.

# 5. Approssimazioni, differenziabilità e derivabilità

$f$  è derivabile in $x_0$ se e solo se $\lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0} = f'(x_0) \in \R$, ossia se $\lim_{x\to x_0}\frac{f(x)-f(x_0)-f'(x_0)(x-x_0)}{x-x_0} = 0$.
Possiamo quindi scrivere le seguenti relazioni.

$$
f(x)-f(x_0)-f'(x_0)(x-x_0)= o(x-x_0), x\to x_0\\
f(x)=f(x_0)+f'(x_0)(x-x_0) +o(x-x_0), x\to x_0\\
f(x)-f(x_0)\sim f'(x_0)(x-x_0) ,x\to x_0
$$

>Definizione: Differenziabilità
>**Data $f:(a,b)\to \R, x_0 \in (a,b)$ diremo che $f$ è differenziabile in $x_0$ se $\exists m\in \R$ tale che $f(x)=f(x_0)+m(x-x_0)+o(x-x_0)$ per $x\to x_0$.**


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Questa è la richiesta che esista un **polinomio di grado al più uno** 
$m(x-x_0)+f(x_0)$ che “approssimi bene” $f(x)$ vicino a $x_0$, nel senso che 
$f(x)-f(x_0)-m(x-x_0)=o(x-x_0), x\to x_0$$\Leftrightarrow$  $\lim_{x\to x_0}\frac{f(x)-f(x_0)-m(x-x_0)}{x-x_0} = 0$.

>Teorema
> **Siano $f:(a,b)\to \R, x_0 \in (a,b)$. Allora $f(x)$ è differenziabile in $x_0$ se e solo se $f$ è ivi derivabile. In tal caso $f(x)= f(x_0)+f'(x_0)(x-x_0)+o(x-x_0)$**
> 

## 5.1 Dimostrazione

1. $f \text{ derivabile} \Rightarrow f \text{ differenziabile, con }m = f'(x_0)$ per definizione di derivata e di retta tangente
2. $f \text{ differenziabile in }x_0$ 
    
    $\Rightarrow$ $\exists m \in \R: f(x)=f(x_0)+m(x-x_0)+o(x-x_0)$
    
    $\Rightarrow \frac{f(x)-f(x_0)}{x-x_0} = m +\frac{o(x-x_0)}{x-x_0}$
    
    $\Rightarrow m = \frac{f(x)-f(x_0)}{x-x_0} +\frac{o(x-x_0)}{x-x_0}$
    
    $\Rightarrow \lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0} = m \in \R$ $\Rightarrow$  $f \text{ è derivabile in }x_0 \text{ e } m = f'(x_0)$
    

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Derivabilità e differenziabilità di $f:(a,b)\to\R$ in $x_0 \in (a,b)$ sono tra loro **equivalenti**. 

Parlare di derivabilità significa interessarsi al tasso di **variazione** **istantanea** di $y = f(x)$ in $x_0$.

Parlare di differenziabilità significa interessarsi al problema di **approssimazione** di $f$ con un polinomio di grado al più uno.


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazioni**

- Le due nozioni **non sono tra loro equivalenti per funzioni di più variabili**;
- Il **miglior polinomio di grado al più uno** che approssima $f$ per $x\to x_0$ è l’equazione della **retta tangente.**

# 6. Punti di non derivabilità

Sia $f:(a,b) \to \R, x_0\in (a,b)$ e $f$ continua in $x_0$.

## 6.1 Punto angoloso

>Definizione: Punto angoloso
**Se $\exists$  finito $\lim_{h\to 0}\frac{f(x_o+h)-f(x_0)}{h}\in \R$, ma $f'_+(x_0)\ne f'_-(x_0)$, allora diremo che $x_0$ è punto angoloso per $f$**


![image.png](17%20Introduzione%20alle%20derivate/image.png)

## 6.2 Punto di flesso a tangente verticale

![image.png](17%20Introduzione%20alle%20derivate/image%201.png)

>Definizione: Punto di flesso
**Se $\exists$  infinito $\lim_{h\to 0}\frac{f(x_o+h)-f(x_0)}{h}= \pm \infty$ diremo che $x_0$ è punto di flesso a tangente verticale per $f$. $x= x_0$ è la retta tangente al grafico in $P(x_0,f(x_0))$.**


## 6.3 Punto di cuspide

>Definizione: punto di cuspide
**Se $\exists$  infiniti e discordi in segno $f'_+(x_0)$ e $f'_-(x_0)$, allora diremo che $x_0$ è punto di cuspide per $f$.**


![image.png](17%20Introduzione%20alle%20derivate/image%202.png)