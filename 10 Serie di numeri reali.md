# 10. Serie di numeri reali

Tags: Serie
Data lezione: 16/10/2024

# 1. Somme parziali, serie, convergenza e carattere

>Definizione: Serie
>**Data una successione di numeri reali $a_n$, definiamo successione delle somme parziali di $a_n$ $S_N=\sum_{n=0}^N a_n= a_0+a_1+...+a_N, \forall N\in \mathbb{N}$. Chiamiamo serie degli $a_n$ la scrittura formale $\sum_{n=0}^{+\infty} a_n$, che formalmente indica la somma degli infiniti termini $a_n$. Diremo che la serie converge a $s\in \mathbb{R}$ se $\exists \lim_{N\to \infty}S_N=s$ e scriveremo $\sum_{n=0}^{+\infty} a_n = \lim_{N\to \infty}S_N = s \in \mathbb{R}$. Diremo che la serie diverge a $\pm \infty$ se $\exists \lim_{N\to \infty}S_N=\pm \infty$ e scriveremo $\sum_{n=0}^{+\infty} a_n = \lim_{N\to \infty}S_N = \pm \infty$. Nel primo caso diremo che $s\in \mathbb{R}$ è la somma della serie, nel secondo caso che $\pm \infty$ è la somma della serie. In ambedue i casi - ossia se $\exists \lim_{N\to \infty}S_N=s \in \overline \mathbb{R}$ diremo che la serie è regolare. Altrimenti, diremo che essa è irregolare o indeterminata.**

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazioni**

- La somma della serie è $s= \sum_{n=0}^{+\infty} a_n = \lim_{N\to \infty}S_N=s \in \overline \mathbb{R}$
- $S_N= \sum_{n=0}^{N-1} a_n + a_{N} = S_{N-1}+a_N ,\forall N$, con $s_0= a_0$

Studiare il **carattere** di una serie significa stabilire se essa converga, diverga o sia irregolare. Ammesso che essa sia convergente, calcolare $\sum_{n=0}^{+\infty} a_n \in \mathbb{R}$ è in generale un problema molto difficile, soprattutto essendo difficile trovare una forma esplicita di $S_N = \sum_{n=0}^{N} a_n$. Diventa pertanto fondamentale determinare condizioni necessarie o sufficienti affinché una serie converga o diverga. Dopo aver determinato ciò è possibile provare a calcolare un valore approssimato della somma.

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Studiare una serie coinvolge sempre **due** **successioni**: $a_n$ e $S_N$.


I **primi** $n_0\in \mathbb{N}$ termini della successione sono **ininfluenti** **per determinare il carattere** della serie. Di contro, se la serie converge, allora **tutti** i termini sono **rilevanti** **per stabilire il valore** di $s= \sum_{n=0}^{+\infty} a_n\in \mathbb{R}$. Inoltre, in una serie, i termini della stessa vanno sommati nel giusto **ordine**, senza alterarlo.

# 2. Serie geometrica di ragione $q$

>Definizione: serie geometrica
>**Data la progressione geometrica $a_n = q^n, n\in \mathbb{N}$, definiamo la serie geometrica nel seguente modo: $\sum_{n=0}^{+\infty} a_n = \sum_{n=0}^{+\infty} q^n$**

Si dimostra che è $S_N=\frac{1-q^{N+1}}{1-q}$ nel caso in cui la ragione sia $\neq$ da 1; se la ragione fosse = 1, allora si tratterebbe di una serie nella forma $\sum_{n=0}^{+\infty}1 = 1+1+1+...=+\infty$.

Come per la progressione geometrica - vista in [7. Successioni e introduzione ai limiti](7%20Successioni%20e%20introduzione%20ai%20limiti%2011334a78851580b9b79fcb0887cf2531.md), paragrafo 2.10 - anche il valore della somma della serie geometrica di ragione $q$ **varia** a seconda del valore della **ragione**. Infatti si ha $\sum_{n=0}^{+\infty} q^n = \lim_{n\to \infty}S_N=\begin{cases}+\infty, & q>1 \\{1\over {1-q}}, & |q|<1\\\nexists, &q < -1\end{cases}$

## 2.1 Dimostrazione

$a_n = q^n \Rightarrow \sum_{n=0}^{+\infty} a_n = \sum_{n=0}^{+\infty} q^n$

Consideriamo ora $S_N = \sum_{n=0}^{N} q^n = 1+q+q^2+...+q^N$ e $qS_{N} = \sum_{n=0}^{N} q^{n+1} = q+q^2+...+q^N+q^{N+1}$ .

$S_N-qS_N=S_N(1-q)=1-q^{N+1}$, cancellandosi i vari termini delle sommatorie tra loro e rimanendo solo il primo e l’ultimo.

È possibile concludere quindi che $S_N=\frac{1-q^{N+1}}{1-q}$.

# 3. Considerazioni sulle serie basate sul teorema dell’algebra dei limiti

Date $\sum_{n=0}^{+\infty} a_n$ e $\sum_{n=0}^{+\infty} b_n$, $\alpha, \beta \in \mathbb{R}$ si può dimostrare applicando la definizione di serie e le proprietà della sommatoria che
$\sum_{n=0}^{+\infty}(\alpha a_n + \beta b_n) = \alpha\sum_{n=0}^{+\infty} a_n+\beta\sum_{n=0}^{+\infty} b_n$ nel caso in cui $\sum_{n=0}^{+\infty} a_n$ e $\sum_{n=0}^{+\infty} b_n$ siano indifferentemente convergenti oppure divergenti e il termine a destra dell’uguale non sia una forma di indeterminatezza.

# 4. Serie telescopiche
>Definizoine: Serie Telescopiche
>**Prendono il nome di serie telescopiche tutte le serie nella forma $\sum_{n=0}^{+\infty} a_n$,  con  $a_n = b_n-b_{n+1}$.**

Sostituendo $a_n$ e sviluppando la sommatoria si dimostra che che $S_N = b_0-b_{N+1}$, in maniera molto simile a quanto fatto nella dimostrazione sulle serie geometriche. Di conseguenza è possibile dedurre che $\exists \lim_{N\to\infty} S_N=\sum_{n=0}^{+\infty} a_n \Leftrightarrow \exists\lim_{N\to\infty}b_N= b^* \in \overline\mathbb{R}$.
Possiamo quindi dedurre che $\sum_{n=0}^{+\infty} a_n  = b_0-b^*.$

Un esempio di serie telescopica è la **serie di Mengoli** $\sum_{n=0}^{+\infty} \frac{1}{n(n+1)}$, dove $\frac{1}{n(n+1)} = \frac{1}{n} -\frac{1}{n+1}.$

# 5. Condizione necessaria per la convergenza di una serie
>Teorema: Condizione necessaria per la convergenza
> **Se $\sum_{n=0}^{+\infty} a_n$  converge $\Rightarrow$  $\lim_{n\to\infty} a_n = 0$.**
> 

Dal teorema precedente segue il seguente corollario, semplicemente assumendo come ipotesi la negazione della tesi e la tesi come negazione dell’ipotesi.

>Corollario
> **$\lim_{n\to\infty} a_n \ne 0$ o $\nexists\lim_{n\to\infty} a_n$ $\Rightarrow$$\sum_{n=0}^{+\infty} a_n$  non converge.**
> 

Qualsiasi serie di una successione divergente o di una successione che ha limite $\ell\ne 0$ non potrà mai convergere.

## 5.1 Dimostrazione

Sia $\sum_{n=0}^{N} a_n = S_N$. Per ipotesi, convergendo la serie, sappiamo che esiste il limite delle somme parziali ed è un numero finito $s\in \mathbb{R}$. Osserviamo, utilizzando le proprietà delle sommatorie che $S_N=\sum_{n=0}^{N-1} a_n  + a_N=S_{N-1}+a_N \Rightarrow a_N=S_N-S_{N-1}$. Per l’algebra dei limiti è possibile dimostrare che $\lim_{N\to\infty} S_N = \lim_{N\to\infty} S_{N-1} = s\in\mathbb{R}$. $\lim_{N\to\infty} a_N = \lim_{N\to\infty} S_N - \lim_{N\to\infty} S_{N-1} = s -s = 0$

---

Osserviamo che il teorema appena scritto **NON** **vale** **“al rovescio”,** pertanto $\lim_{n\to\infty} a_n = 0$ $\nRightarrow$  $\sum_{n=0}^{+\infty} a_n$  converge e un esempio può essere fornito dalla **serie armonica, $\sum_{n=0}^{+\infty} \frac{1}{n}$ ,** in cui il limite di $a_n$ tende effettivamente a 0, ma ha carattere divergente.

# 6. Resto *N-esimo* della serie
>Definizione
> **Data una serie $\sum_{n=0}^{+\infty} a_n$ , se essa converge, diverge o è indeterminata, $\Rightarrow$$\forall N\in \mathbb{N}$, la serie $R_N = \sum_{n=N+1}^{+\infty} a_n$  rispettivamente converge, diverge o è indeterminata.
Nel caso in cui converga, allora $\lim_{n\to\infty}R_N=0$**
> 

<img src="https://www.notion.so/icons/circle-alternate_red.svg" alt="https://www.notion.so/icons/circle-alternate_red.svg" width="15px" /> **Osservazione**
Se $\sum_{n=0}^{+\infty} a_n$  converge a $s$ $\Rightarrow$ 
$R_N = \sum_{n=N+1}^{+\infty} a_n = \sum_{n=0}^{+\infty} a_n -\sum_{n=0}^{N} a_n  = S-S_N$

>Definizione: Resto ennesimo
>**$R_N=\sum_{n=N+1}^{+\infty} a_n$  prende il nome di resto *N-esimo* della serie $\sum_{n=0}^{+\infty} a_n$** 

Possiamo quindi concludere che, nel caso di serie convergenti, il resto della serie è infinitesimo.