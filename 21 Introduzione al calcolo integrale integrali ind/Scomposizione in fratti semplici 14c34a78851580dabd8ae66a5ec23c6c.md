# Scomposizione in fratti semplici

---

Nota: pagina realizzata con l’ausilio di ChatGPT.

---

La **scomposizione in fratti semplici** è una tecnica fondamentale per calcolare integrali del tipo  $\int \frac{P(x)}{Q(x)} \, dx$ , dove $P(x)$ e $Q(x)$ sono polinomi. L’idea di base è riscrivere il rapporto $\frac{P(x)}{Q(x)}$ come somma di termini più semplici (i **fratti semplici**), che siano più facili da integrare.

# **1. Verificare il grado di**  $P(x)$  **e**  $Q(x)$

Se il grado di  $P(x)$  $( \deg(P) )$ è **maggiore o uguale** al grado di $Q(x) ( \deg(Q) )$, esegui la **divisione polinomiale**. Questo produce un quoziente $Q(x)$e un resto  $R(x)$ tali che
$\frac{P(x)}{Q(x)} = T(x) + \frac{R(x)}{Q(x)},$ dove $T(x)$ è un polinomio e $\deg(R) < \deg(Q)$. 
L’obiettivo è quindi concentrarsi su $\frac{R(x)}{Q(x)}$ .

# **2. Scomposizione del denominatore** $Q(x)$

Fattorizza $Q(x)$ nel prodotto di polinomi **irriducibili** (su  $\mathbb{R}$ ) e scrivi  $\frac{R(x)}{Q(x)}$ come somma di fratti semplici. Si possono verificare i seguenti casi per i fattori di $Q(x)$:

1. **Fattori lineari distinti**:  $(x - a_1)(x - a_2)\cdots(x - a_n)$.
2. **Fattori lineari ripetuti**:  $(x - a)^m$ .
3. **Fattori quadratici irriducibili distinti**:  $(x^2 + px + q)$, con $\Delta < 0$ .
4. **Fattori quadratici irriducibili ripetuti**:  $(x^2 + px + q)^m$, con $\Delta < 0$ .

# **3. Costruire i fratti semplici:**

A seconda dei fattori di $Q(x)$, l’algoritmo procede in maniera differente.

## **Fattori lineari distinti**  $(x - a_i)$

$$
\frac{R(x)}{Q(x)} = \frac{A_1}{x - a_1} + \frac{A_2}{x - a_2} + \cdots + \frac{A_n}{x - a_n}
$$

## **Fattori lineari ripetuti**  $(x - a)^m$

$$
\frac{B_1}{x - a} + \frac{B_2}{(x - a)^2} + \cdots + \frac{B_m}{(x - a)^m}
$$

## **Fattori quadratici irriducibili distinti** $x^2 + px + q$

$$
\frac{Cx + D}{x^2 + px + q}
$$

## **Fattori quadratici irriducibili ripetuti** $(x^2 + px + q)^m$

$$
\frac{E_1x + F_1}{x^2 + px + q} + \frac{E_2x + F_2}{(x^2 + px + q)^2} + \cdots + \frac{E_mx + F_m}{(x^2 + px + q)^m}
$$

# **4. Determinare le costanti**

Per calcolare le costanti $( A_i, B_i, C, D, E_i, F_i )$, risolvi un sistema di equazioni derivato uguagliando il numeratore di $\frac{P(x)}{Q(x)}$ con il numeratore della somma dei fratti semplici.

# **5. Integrare i termini**

Una volta trovati i fratti semplici, integra ciascun termine. È molto comune trovare un’espressione del tipo $\int \frac{1}{x - a} \, dx = \ln|x - a| + c$, oppure una derivata che può essere ricondotta a quella dell’arctangente, ad esempio nella forma $\int \frac{1}{a^2 +x^2}$.

Nel caso di $\int \frac{Cx + D}{x^2 + px + q} \, dx$ bisogna invece cercare di completare il quadrato al denominatore per integrare termini nelle forme  $\frac{1}{x^2 + a^2}$  o  $\frac{x}{x^2 + a^2}$ .