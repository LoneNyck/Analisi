# 9. Confronti e stime asintotiche per successioni

Tags: Limiti, Successioni
Data lezione: 09/10/2024

# 1. Ordine di infiniti e infinitesimi

## 1.1 Ordine di infiniti

Siano $a_n$  e $b_n$ successioni **infinite**, $b_n \neq 0$ definitivamente.

- $\lim_{n\to\infty}\frac{a_n}{b_n} = 0 \Rightarrow$ $a_n$ è infinito di **ordine inferiore** rispetto a $b_n$.
- $\lim_{n\to\infty}\frac{a_n}{b_n} = l\in\mathbb{R}\setminus\{0\} \Rightarrow$ $a_n$ e $b_n$ sono infiniti dello **stesso ordine.**
- $\lim_{n\to\infty}\frac{a_n}{b_n} = \pm \infty \Rightarrow$ $b_n$ è infinito di **ordine inferiore** rispetto a $a_n$.
- $\nexists\lim_{n\to\infty}\frac{a_n}{b_n}  \Rightarrow$ $a_n$, $b_n$ sono infiniti, ma **non** sono **confrontabili.**

## 1.2 Ordine di infinitesimi

Siano $a_n$  e $b_n$ successioni **infinitesime**, $b_n \neq 0$ definitivamente.

- $\lim_{n\to\infty}\frac{a_n}{b_n} = 0 \Rightarrow$ $a_n$ è infinitesimo di **ordine superiore** rispetto a $b_n$.
- $\lim_{n\to\infty}\frac{a_n}{b_n} = l\in\mathbb{R} -\{0\} \Rightarrow$ $a_n$ e $b_n$ sono infinitesimi dello **stesso ordine.**
- $\lim_{n\to\infty}\frac{a_n}{b_n} = \pm \infty \Rightarrow$ $b_n$ è infinito di **ordine superiore** rispetto a $a_n$.
- $\nexists\lim_{n\to\infty}\frac{a_n}{b_n}  \Rightarrow$ $a_n$, $b_n$ sono infinitesimi, ma **non** sono **confrontabili.**

# 2. Asintotico ed $o$-*piccolo*

>Definizione: o-piccolo e asintotico 
>**Date $a_n, b_n$, con $b\neq0$  definitivamente, diremo che** 
>- **$a_n$ è $o$-*piccolo* di $b_n$  e scriveremo $a_n = o(b_n)$ per $n\to \infty$ se
>$\lim_{n\to\infty}\frac{a_n}{b_n}= \lim_{n\to\infty}\frac{o(b_n)}{b_n} = 0$**
>- **$a_n$ è asintotico a $b_n$  e scriveremo $a_n \sim b_n$ per $n\to \infty$ se $\lim_{n\to\infty}\frac{a_n}{b_n}=1$**

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**

- $\lim_{n\to\infty}\frac{a_n}{b_n}=\pm\infty$ $\Rightarrow$ $\lim_{n\to\infty}\frac{b_n}{a_n}=0$ $\Rightarrow$  $b_n = o(a_n)$
- $\lim_{n\to\infty}\frac{a_n}{b_n}=\ell\in\mathbb{R}-\{0\}$ $\Rightarrow$  $\lim_{n\to\infty}\frac{a_n}{\ell b_n}=1$ $\Rightarrow$ $a \sim\ell b_n$

È possibile dimostrare che valgono le seguenti proprietà per la relazione di asintotico:

1. $a_n \sim a_n$ (**riflessività**)
2. $a_n \sim b_n$ e $b_n \sim c_n$ $\Rightarrow$ $a_n \sim c_n$ (**transitività**)
3. $a_n\sim b_n \Rightarrow b_n \sim a_n$ (**commutatività**)

Possiamo quindi concludere che  $\sim$ è una **relazione di equivalenza** tra le successioni.

Inoltre è possibile stabilire una relazione tra $o$-*piccolo* e asintotico:

$$
{a_n \sim b_n \Leftrightarrow a_n = b_n + o(b_n)\Leftrightarrow a_n - b_n = o(b_n)}
$$

## 2.1 Un nuovo modo per vedere la gerarchia degli infiniti

- $(\log_a n)^\beta = o(n^\alpha)$, $\forall a> 1, \alpha > 0, \beta >0$
- $n^\alpha=o(a^n)$, $\forall a >1, \alpha >0$
- $a^n=o(n!)$
- $n! = o(n^n)$

# 3. Proposizioni sugli asitotici

- Se $a_n \sim a_n'$ e $b_n \sim b_n'$ $\Rightarrow$  $a_nb_n \sim a_n'b_n'$
- Se $a_n \sim a_n'$ e $b_n \sim b_n'$ $\Rightarrow$  $\frac{a_n}{b_n} \sim \frac{a_n'}{b_n'}$
- Se $a_n \sim a_n'$ $\Rightarrow$  $(a_n)^\alpha \sim (a_n')^\alpha$
- Se $a_n \sim a_n'$ $\Rightarrow$  $a_n$ e $a_n'$ hanno lo **stesso** **carattere**, ossia o convergono entrambi allo stesso limite, o divergono ambedue a $+\infty$ o $-\infty$ oppure sono irregolari

La relazione di asintotico può quindi essere usata senza limitazioni per quanto riguarda **prodotti**, **rapporti** e **potenze**.

In generale, date $a_n\sim a_n'$ e  $b_n\sim b_n'$ senza specificare ulteriori condizioni:

1. $a_n\pm b_n \nsim a_n'\pm b_n'$
2. $(a_n)^{b_n} \nsim (a_n')^{b_n'}$
3. $e^{a_n} \nsim e^{a_n'}$
4. $\log a_n \nsim \log a_n'$

La relazione di asintotico **NON** vale quindi per la **somma**, per **l’esponenziale** e per il **logaritmo** a meno di ulteriori condizioni.

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazioni**

1. $a_n \sim b_n \nRightarrow a_n-b_n \to 0$
2.  $a_n-b_n \to 0 \nRightarrow a_n \sim b_n$ 

La relazione di asintotico può essere usata anche con **funzioni** **composte**, partendo però da quella più esterna, per arrivare a quella più interna. 

# 4. Considerazioni sugli $o$-piccoli

Segue una serie di considerazioni sugli $o$-piccoli:

- $a_n o(b_n) = o(a_nb_n)$, ossia il prodotto per una successione scala dentro l’*o-piccolo*;
- $c\cdot o(a_n) = o(a_n)$, ossia il prodotto per uno scalare è ininfluente;
- $\pm o(a_n) = o(a_n)$, ossia il segno è ininfluente;

- $o({1\over n}) + o({1\over n^2}) = o({1\over n})$ , ossia per gli infinitesimi vince quello più grande, cioè quello di denominatore minore;
- $o(n) + o(n^2) = o(n^2)$, ossia per gli infiniti vince quello di grado più grande;
- $a_n \sim b_n \Rightarrow o(a_n) \sim o(b_n)$, ossia se due successioni sono asintotiche, anche i relativi *o-piccoli* saranno asintotici.