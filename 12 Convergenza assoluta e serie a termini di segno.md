# 12. Convergenza assoluta e serie a termini di segno variabile

Tags: Serie
Data lezione: 23/10/2024

# 1. Convergenza assoluta

> Definizione: Convergenza assoluta
> **Data una serie $\sum_{n=1}^{+\infty} a_n$, diremo che essa converge assolutamente se $\sum_{n=0}^{+\infty} |a_n|$ converge, ossia $\exist \lim_{N\to\infty}\sum_{n=0}^{N} |a_n| = M \in \R$.**

Per distinguere questa nuova definizione di convergenza da quella data in precedenza in [10. Serie di numeri reali](10%20Serie%20di%20numeri%20reali%2012134a7885158025ab5eda4c4a2cb72b.md), par. 1, chiameremo la vecchia nozione di convergenza “**convergenza semplice**”.

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazioni**

- Una serie $\sum_{n=0}^{+\infty} |a_n|$ converge oppure diverge a $+\infty$, essendo a termini positivi.
- Se una **serie** a **termine positivi** converge semplicemente $\Leftrightarrow$  converge assolutamente; si noti che se la serie non è a termini positivi, questa relazione non vale.

# 2. Criterio della convergenza assoluta
>Teorema: Criterio della convergenza assoluta
> **Se $\sum_{n=0}^{+\infty} a_n$ converge assolutamente, allora essa converge semplicemente. In tal caso, inoltre, $|\sum_{n=0}^{+\infty} a_n| \le \sum_{n=0}^{+\infty} |a_n|$.**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**

- **Convergenza assoluta $\Rightarrow$  convergenza semplice**
- **Convergenza semplice $\nRightarrow$  convergenza assoluta**

Da quest’ultima osservazione possiamo dedurre che esistono delle serie che convergono semplicemente ma non assolutamente. Un esempio, che può essere verificato con il criterio di Leibniz che vedremo in seguito, è $\sum_{n=0}^{+\infty}\frac{(-1)^n}{n^\alpha}, 0< \alpha \le 1$.

Poiché $\sum_{n=0}^{+\infty} |a_n|$ è una serie a termini positivi, possono essere usati tutti i criteri visti in [11. Serie a termini definitivamente “positivi”](11%20Serie%20a%20termini%20definitivamente%20%E2%80%9Cpositivi%E2%80%9D%2012134a78851580ecafbef6bb3636d4ff.md) per provarne la convergenza. 

# 3. Serie a termini di segno alterno

> Definizione: Serie a termini di segno alterno
>**Una serie si dice a termini di segno alterno se ha la forma $\sum_{n=0}^{+\infty} (-1)^n a_n, a_n > 0$**


## 3.1 Criterio di Leibniz
>Teorema: Criterio di Leibniz
> **Data la serie a termini di segno alterno $\sum_{n=0}^{+\infty} (-1)^n a_n$ tale che**
> 
> 1. **$a_n \ge 0$ definitivamente,**
> 2. **$a_n$ sia decrescente, ossia $a_{n+1} \le a_n$,**
> 3. **$\lim_{n\to\infty}a_n = 0$,**
> 
> **allora $\sum_{n=0}^{+\infty} (-1)^n a_n$ converge semplicemente.**
> 

Inoltre se $S = \sum_{n=0}^{+\infty} (-1)^n a_n$, allora:

1. $S_{2N} = \sum_{n=0}^{2N} (-1)^n a_n$ $\downarrow S$ (ossia la serie limitata da un numero pari si avvicina a S dall’alto)
2. $S_{2N+1} = \sum_{n=0}^{2N+1} (-1)^n a_n$ $\uparrow S$ (ossia la serie limitata da un numero dispari dei termini si avvicina a S dal basso)
3. $|R_N| = |S-S_N| = |\sum_{n=N+1}^{+\infty} (-1)^n a_n| \le a_{N+1}$ $\forall N \in \N$

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**

- Non si può rimuovere dal criterio di Leibniz l’ipotesi di decrescenza.
- $a_n \sim b_n,\ a_n, b_n> 0, \ \sum_{n=0}^{+\infty} (-1)^nb_n$ converge $\nRightarrow$ $\sum_{n=0}^{+\infty} (-1)^n a_n$ converge.
Il criterio del **confronto asintotico** infatti vale **SOLO** per serie a termini **definitivamente** **positivi** e non per serie a termini di segno alterno.
- $a_n \sim b_n$ e $b_n$ monotona $\nRightarrow$ $a_n$ monotona.
Infatti **l’asintotico** è una relazione di equivalenza e **non** **trasmette la monotonia** come invece trasmette il segno.

### 3.1.1 Dimostrazione

Proviamo a dimostrare l’osservazione appena fatta costruendo due successioni $a_n$ e $b_n$ tali che:

1. $a_n,b_n \ge 0$
2. $a_n \sim b_n$
3. $\lim_{n\to\infty}a_n = \lim_{n\to\infty}b_n = 0$
4. $b_n$ sia decrescente

Da quanto appena detto consegue che $\sum_{n=0}^{+\infty} (-1)^nb_n$ converge semplicemente per il criterio di Leibniz.

v.   $\sum_{n=0}^{+\infty} (-1)^na_n$ diverge, quindi $a_n$ non può essere decrescente perché se lo fosse rispetterebbe tutte le condizioni del criterio di Leibniz

Costruiamo le successioni nel seguente modo $b_n = \frac{1}{\sqrt{n}}$ e $a_n = \frac{\sqrt{n}+(-1)^n}{n}$ - si noti che non si tratta dell’unica scelta valida.

Le condizioni i. , ii. , iii. , iv. sono facilmente verificabili. La v. si dimostra svolgendo il prodotto, spezzando la frazione e dividendo la sommatoria (che può essere fatto non trattandosi di una forma di indeterminatezza).