# 2. Panoramica su teoremi, dimostrazioni e controesempi

Tags: Teoremi e dimostrazioni\
Data lezione: 18/09/2024

# 1. Definizioni

>Definizone: Teorema\
>**Un teorema è un asserto di cui si vuole dimostrare la verità partendo da delle ipotesi assunte vere.
>Le ipotesi sono una o più proposizioni o predicati.
>Dimostrare un teorema significa dimostrare che $P \Rightarrow Q$ è vera oppure egualmente che $\neg Q \Rightarrow \neg P$ è vera.**

>Definizione: Dimostrazione\
>**La dimostrazione è l’insieme di passaggi che portano da una proposizione all’altra, che ha come partenza $P$ vera e come arrivo $Q$ vera.**

# 2. Metodi delle dimostrazioni

## 2.1 Metodo deduttivo diretto

Sfrutta la definizione di teorema,  cercando pertanto di dimostrare che $P \Rightarrow Q$.

## 2.2 Variante del metodo deduttivo diretto

Sfrutta anch’esso la definizione di teorema, utilizzando però la negazione della tesi, cercando quindi di dimostrare che $\neg Q \Rightarrow \neg P$

## 2.3 Controesempio

Utilizzato per smentire un teorema, cerca di sfruttare il fatto che $P \Rightarrow Q$  sia falsa quando $P$ è vera e $Q$ è falsa.

Per un’implicazione universale, mostrare che essa sia falsa significa mostrare che $\exists x_0 \in A : P(x_0) \Rightarrow Q(x_0)$ sia falsa e $x_0$ prende il nome di **controesempio**. 

## 2.4 Dimostrazione per assurdo

Per dimostrare la verità di $P \Rightarrow Q$ si può assumere che $P$ sia vera e $Q$  sia falsa, ossia che $\neg Q$ sia vera.  $\neg Q$ prende il nome di **ipotesi di assurdo**.

A questo punto tramite dimostrazione diretta si cerca di giungere ad una contraddizione.

$P \wedge Q   \Rightarrow contr. \Rightarrow P \wedge Q \, falsa \Rightarrow\neg Q \, falsa \Rightarrow Q \, vera$

## 2.5 Dimostrazione per induzione

Utilizzata per dimostrare la verità di un’implicazione universale nella forma $\forall n \in \mathbb{N} , P(n)$ è vera. Si articola in due passi:

1. $P(0)$ è vera
2. $P(n+1)$  è vera se $P(n)$ è vera $\forall n \in \mathbb{N}$, che si traduce in $\forall n \in \mathbb{N}, P(n) \Rightarrow P(n+1)$, dove $P(n)$ prende il nome di **ipotesi di induzione**
