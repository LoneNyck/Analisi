# 24. Funzioni integrali e Teorema fondamentale del calcolo integrale II

Tags: Dimostrazione importante, Integrali
Data lezione: 12/12/2024

# 1. Funzioni integrali

>Definizione
**Sia $f:I\subseteq \R\to \R$, con $I$  intervallo, $f$ Riemann integrabile in $I$  in senso proprio o improprio indifferentemente. Sia $x_0 \in I$.**
>
>$$
>F(x) = \int_{x_0}^xf(t)\ dt, \forall x\in I
>$$
>**$F$ prende il nome di funzione integrale di $f$.**


# 2. Teorema fondamentale del calcolo integrale
>Teorema
> **Sia $f:[a,b]\to \R$ Riemann integrabile in senso proprio o improprio indifferentemente in $[a,b]$. Sia $x_0 \in [a,b]$. Consideriamo $F(x) = \int_{x_0}^xf(t)\ dt, \forall x\in I$.
Allora vale che:**
> 
> 1. **$F$ è continua in $[a,b]$**
> 2. **Se $f$ è continua in $\overline x\in [a,b]$, allora $F$ è derivabile in $\overline x$ e vale $F'(\overline x) = f(\overline x)$**

### 2.1 Dimostrazione

1. Consideriamo $f:[a,b]\to \R$ Riemann integrabile in senso proprio.
    
    Allora $f$ deve essere limitata in $[a,b]$, ossia $\exists M >0: |f(x)|\le M$ . Sia $\overline x \in [a,b]$, $h\in \R:x+h\in [a,b]$.
    Per $h> 0$ abbiamo che
    
    $$
    |F(x+h)- F(x)| = |\int_{x_0}^{x+h}f(t) \ dt -\int_{x_0}^{x}f(t) \ dt |= \\
    =|\int_{x_0}^{x+h}f(t) \ dt +\int_{x}^{x_0}f(t) \ dt | = \\
    =|\int_{x}^{x+h}f(t) \ dt|
    $$
    
    Per monotonia dell’integrale vale che $|\int_{x}^{x+h}f(t) \ dt|\le \int_{x}^{x+h}|f(t)| \ dt \le \int_{x}^{x+h}M dt$
    
    Possiamo quindi concludere che $|F(x+h)- F(x)| \le M h$.
    
    Similmente per $h< 0$ vale che $|F(x+h)- F(x)| \le M |h|$.
    
    Di conseguenza $\forall h \in \R, |F(x+h)- F(x)| \le M |h|$, pertanto per confronto possiamo scrivere che $\lim_{h\to0}|F(x+h)- F(x)| \le \lim_{h\to0} M |h|=0$, e per teorema del confronto vale che $\lim_{h\to0}|F(x+h)- F(x)|=0$, quindi
    $\lim_{h\to0}F(x+h)= F(x)$ e $F$  è continua per definizione.
    
2. Consideriamo $f$ continua ovunque e cerchiamo di dimostrare che $F$ è derivabile ovunque e $F'(x) = f(x)$.
    
    Sia $x \in [a,b]$, $h\in \R:x+h\in [a,b]$. Come visto sopra vale che 
    $F(x+h)- F(x)= \int_{x}^{x+h}f(t) \ dt$, quindi deve valere anche che
    
    $$
    \frac{F(x+h)- F(x)}{h}= \frac{\int_{x}^{x+h}f(t) \ dt}{h}
    $$
    
    Poiché $f$ è continua ovunque, per $h>0$  abbiamo che $\frac{\int_{x}^{x+h}f(t) \ dt}{h}$ è il valor medio di $f$ in $[x,x+h]$ per il teorema della media integrale, quindi $\exists x_h\in [x,x+h]:\\f(x_h)= \frac{\int_{x}^{x+h}f(t) \ dt}{h}$.
    
    Allora $\frac{F(x+h)- F(x)}{h}= \frac{\int_{x}^{x+h}f(t) \ dt}{h}= f(x_h)$.
    
    Per confronto vale che $\lim_{h\to 0^+}x_h= x$, mentre per continuità di $f$ possiamo scrivere che $\lim_{h\to 0}f(x_h)= f(\lim_{h\to 0}x_h) = f(x)$.
    
    Allora $\lim_{h\to 0^+}\frac{F(x+h)- F(x)}{h}=\lim_{h\to 0^+} f(x_h)= f(x)$.
    
    In maniera simile si può dimostrare che $\lim_{h\to 0^-}\frac{F(x+h)- F(x)}{h}=\lim_{h\to 0^-} f(x_h)= f(x)$
    
    Allora vale che $F'(x) =\lim_{h\to 0}\frac{F(x+h)- F(x)}{h}= f(x)$.
    


>Corollario
> **Sia $f:[a,b]\to \R$ continua. Allora essa è Riemann integrabile in $[a,b]$ ed ammette primitiva in $[a,b]$ $F(x) = \int_a^xf(t)\ dt + c$.**
> 
> 
> **Inoltre $\int_a^b f(x)\ dx=G(b)-G(a)$, dove $G$ è una primitiva qualsiasi di $f$.**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Si tratta del Teorema fondamentale del calcolo I, visto in [22. Integrale di Riemann, Teorema della media integrale e Teorema fondamentale del calcolo integrale I](<23 Integrale di Riemann generalizzato e criteri di convergenza.md>), per funzioni continua.


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Se $f:\R\to \R$ è continua e $\phi :\R\to \R$ è derivabile, per il teorema fondamentale del calcolo integrale II e il teorema di derivazione delle funzioni composte vale che

$$
G(x) = \int_{x_0}^{\phi(x)}f(t) \ dt \text{ è derivabile e }\\G'(x) = f(\phi(x))\cdot\phi'(x)
$$