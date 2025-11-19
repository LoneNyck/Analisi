# 8. Calcolo dei limiti per successioni e numero di Nepero

Tags: Limiti, Successioni

# 1. Teorema sull’algebra dei limiti

>Teorema
>**Siano $a_n$  e $b_n$ due successioni ed $\exists\lim_{n\to\infty}a_n=a\in {\mathbb{R}}$ ed $\exists\lim_{n\to\infty}b_n=b\in {\mathbb{R}}$.
Allora:**
>
>1. **$\lim_{n\to\infty}a_n\pm b_n = a \pm b$**
>2. **$\lim_{n\to\infty}a_nb_b = ab$**
>3. **$\lim_{n\to\infty}{a_n \over b_n} = {a \over b}, b\neq 0$**
>4. **$\lim_{n\to\infty}{a_n}^{b_n}=a^b, a >0$**

La dimostrazione del punto i. è relativamente semplice e fa uso della disuguaglianza triangolare raccogliendo “tutti gli $a$” e “tutti i $b$” e della definizione di limite vista in [7. Successioni e introduzione ai limiti](7%20Successioni%20e%20introduzione%20ai%20limiti%2011334a78851580b9b79fcb0887cf2531.md), al punto 2.2, adottando $\epsilon \over 2$ invece del più consueto $\epsilon$. 

## 1.1 Corollario sull’algebra dei limiti

>Corollario
>**Siano $a_n$  e $b_n$ due successioni ed $\exists\lim_{n\to\infty}a_n=a\in {\mathbb{R}}$ ed $\exists\lim_{n\to\infty}b_n=b\in {\mathbb{R}}$.**
>**Allora:**
>1. **$a>b$ $\Rightarrow$ $a_n>b_n$ definitivamente in $n\in\mathbb{N}$**
>2. **$a_n \ge b_n$ definitivamente in $n \in \mathbb{N}$ $\Rightarrow$  $a\ge b$**

La dimostrazione di ambedue i punti fa utilizzo di una successione $c_n = a_n-b_n$ e dei teoremi di permanenza del segno [[7. Successioni e introduzione ai limiti](7%20Successioni%20e%20introduzione%20ai%20limiti%2011334a78851580b9b79fcb0887cf2531.md), 2.10].

# 2. Teorema del confronto
>Teorema del confronto
> **Date tre successioni $a_n$, $b_n$ e $c_n$ : $a_n \le b_n \le c_n$ definitivamente in $n \in \mathbb{N}$ ed $\exists\lim_{n\to\infty}a_n=\lim_{n\to\infty}c_n=l\in {\mathbb{R}}$
$\Rightarrow$  $\exists \lim_{n\to\infty}b_n = l \in {\mathbb{R}}$**
> 

### 2.0 comma 1 - Dimostrazione

Questo teorema si basa interamente sulla definizione di limite di $a_n$  e $c_n$, per poi utilizzare la disuguaglianza dell’ipotesi per poter dimostrare l’esistenza del limite di $b_n$ e il suo valore.

## 2.1 Teorema del confronto per una funzione che diverge

Dal teorema del confronto è possibile anche dedurre il seguente teorema.
>Teorema
> **Date due successioni $a_n$ e $b_n$ : $a_n \le b_n$  definitivamente in $n \in \mathbb{N}$**
> - **se $a_n$ diverge ed $\exists\lim_{n\to\infty}a_n=+\infty$ 
> $\Rightarrow$  $\exists \lim_{n\to\infty}b_n = +\infty$**
> - **se $b_n$ diverge ed $\exists\lim_{n\to\infty}b_n=-\infty$ 
> $\Rightarrow$  $\exists \lim_{n\to\infty}a_n = -\infty$**

### 2.1.1 Dimostrazione

Come la precedente, anche questo teorema si basa sulla definizione di limite per poi utilizzare la disuguaglianza dell’ipotesi per dimostrare l’esistenza del limite.

## 2.2 Corollario del teorema del confronto

> Corollario
>1. **Date due successioni $a_n$ e $b_n$ : $|a_n| \le |b_n |$ definitivamente in $n \in \mathbb{N}$ ed 
>$\exists\lim_{n\to\infty}b_n=0 \in {\mathbb{R}}$ $\Rightarrow$ $\exists\lim_{n\to\infty}a_n=0 \in {\mathbb{R}}$**
>2. **Date due successioni $a_n$ e $b_n$ tali che $a_n$ sia limitata e $\exists\lim_{n\to\infty}b_n=0$ $\Rightarrow$ $\exists\lim_{n\to\infty}a_nb_n=0$**

### 2.2.1 Dimostrazione

1. Il primo punto del corollario si basa unicamente sulla definizione di disuguaglianza con valore assoluto e sul teorema del confronto;
2. Il secondo punto si basa sul concetto di limitatezza di una successione: $a_n$ limitata $\Rightarrow \exists M > 0 : |a_n| < M, \forall n \in \mathbb{N}$. Moltiplicando per $|b_n|$ da ambedue i lati otteniamo che $|a_nb_n|< M|b_n|$. Sapendo che in $\lim_{n\to\infty}M|b_n|=0$ ci siamo ricondotti al primo punto del corollario, dimostrando pertanto che $\exists\lim_{n\to\infty}a_nb_n=0$

# 3. Gerarchia degli infiniti
>Gerarchia degli infiniti
> **$\lim_{n\to\infty}{\log a_n\over n^\alpha}=0$**
> 
> **$\lim_{n\to\infty}{n^\alpha \over a^n}=0$**
> 
> **$\lim_{n\to\infty}{a^n\over n!}=0$**
> 

Dai limiti appena scritti si può facilmente dedurre che per $n\to \infty$, $\log a_n < n^\alpha<a^n<n!$, relazione che prende il nome di **gerarchia degli infiniti.**

# 4. Aritmetizzazione parziale di infinito e forme di indeterminatezza

Seguono una serie di **regole** per il calcolo dei limiti di successioni. Siano $a_n$  e $b_n$ due successioni qualunque.

1. Se $\lim_{n\to\infty}a_n = \ell \in {\mathbb{R}}$ e $\lim_{n\to\infty}b_n = \pm \infty$
$\Rightarrow$ $\lim_{n\to\infty}a_n+b_n=\pm \infty$
2. Se $\lim_{n\to\infty}a_n = \lim_{n\to\infty}b_n = \pm \infty$ 
$\Rightarrow$ $\lim_{n\to\infty}a_n+b_n=\pm \infty$
3. Se $\lim_{n\to\infty}a_n = \ell \in \overline {\mathbb{R}} \setminus\{0\}$ e $\lim_{n\to\infty}b_n = \pm \infty$
$\Rightarrow$ $\lim_{n\to\infty}a_nb_n=\pm \infty$ con le usuali regole del segno.
4. Se $\lim_{n\to\infty}a_n = \ell \in \overline {\mathbb{R}} \setminus\{0\}$ e $\lim_{n\to\infty}b_n = 0^\pm$
$\Rightarrow$ $\lim_{n\to\infty}{a_n\over b_n}=\pm \infty$ con le usuali regole del segno.
5. Se $\lim_{n\to\infty}a_n = \ell \in {\mathbb{R}}$ e $\lim_{n\to\infty}b_n = \pm \infty$
$\Rightarrow$ $\lim_{n\to\infty}{a_n\over b_n}=0$

Prendono il nome di **forme di indeterminatezza** tutte le seguenti: $\infty-\infty$; $\infty \cdot 0$; $\infty \over \infty$; $0 \over 0$.

## 4.1 Estensione dell’algebra dei limiti

>Teorema 
> **Se $a_b$ e $b_n$ sono successioni $\lim_{n\to\infty}a_n = a \in \overline {\mathbb{R}}, a>0$ e $\lim_{n\to\infty}b_b = b \in \overline {\mathbb{R}}$ $\Rightarrow$ $\lim_{n\to\infty}{a_n}^{b_n}= a^b$.**
> 
1. $a^{+\infty} = +\infty$, $\forall a>1$
2. $a^{-\infty} = 0$, $\forall a>1$
3. $a^{+\infty} = 0$, $0<a<1$
4. $a^{+\infty} = +\infty$, $0<a<1$
5. ${+\infty}^b = 0$, $\forall b >0$
6. ${+\infty}^b = 0$, $\forall b <0$

Sono escluse le **forme d’indeterminatezza**: $\infty^0$, $0^0$, $1^\infty$.

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**

NON sono forme di indeterminatezza le seguenti:

- $a_n=1$ e $b_n =n$ $\Rightarrow$ ${a_n}^{b_n} = 1^n = 1 \to 1$, $n \to \infty$
- $a_n=0$ e $b_n =n$ $\Rightarrow$ ${a_n}^{b_n} = 0^n = 0 \to 0$, $n \to \infty$

# 5. Il numero di Nepero $e$

>Teorema
> **La successione $a_n = (1 + \frac{1}{n})^n$ è monotona crescente e limitata; in particolare essa ammette limite in ${\mathbb{R}}$.**
> 

## 5 comma 1 - Dimostrazione

La dimostrazione si articola in due punti: i. mostrare che $a_n$ è crescente; ii. mostrare che $a_n$ è limitata.

1. Mostrare che una successione è crescente  $a_n \ge a_{n-1}, \forall n\ge2$ $\Rightarrow$ $\frac{a_n}{a_{n-1}}\ge1$, in cui il passaggio fondamentale per la dimostrazione della disuguaglianza è la disuguaglianza di Bernoulli.
2. Per dimostrare che a_n sia limitata introduciamo la successione b_n decrescente : $a_n \le b_n \forall n\in\mathbb{N}, n>1$ $\Rightarrow$ $a_n \le b_n \le b_1 ,\forall n\ge1$. 
$b_n = (1+\frac{1}{n})^{n+1}=a_n(1+\frac{1}{n})$, quindi effettivamente $b_n \ge a_n$. Ora sarà sufficiente dimostrare che $b_n$ è decrescente con il medesimo metodo utilizzato nel punto i, quindi $\frac{b_{n-1}}{b_{n}}\ge1$.

---

> Definizione: Numero di Nepero
>**Definiamo il numero di Nepero $e= \lim_{n\to\infty}(1 + \frac{1}{n})^n$**


<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Il numero di Nepero può essere anche visto come l’estremo superiore di $a_n$.


## 5.1 Teorema (conseguenza della definizione di $e$)

>Teorema
> **Sia $c_n$ una successione tale che $\lim_{n\to\infty}c_n = \pm \infty$. Allora $\lim_{n\to\infty}(1 + \frac{1}{c_n})^{c_n} = e$**
> 

## 5.2 Corollario (conseguenza della definizione di $e$)
>Corollario
> **$$\forall a \in {\mathbb{R}}, \lim_{n\to\infty}(1 + \frac{a}{n})^n = e^a$$**
> 

# 6. Criterio del rapporto tra successioni

>Teorema: criterio del rapporto tra successioni
> **Sia $a_n$ una successione tale che $a_n >0$ definitivamente e $\exists \ell=\lim_{n\to\infty}\frac{a_{n+1}}{a_n}\in \overline{\mathbb{R}}$.**
> 
> - **$\ell > 1 \Rightarrow \lim_{n\to\infty}a_n=+\infty$;**
> - **$0< \ell < 1 \Rightarrow \lim_{n\to\infty}a_n=0$;**
> - **$\ell = 1 \Rightarrow$  non si può dire nulla sul limite di $a_n$**

## 6.1 Estensione della gerarchia degli infiniti

$$
(\log_an)^\beta \ll n^\alpha \ll a^n \ll n! \ll n^n, \forall a>1, \beta >0, \alpha >0 
$$