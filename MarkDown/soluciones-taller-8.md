# Algunas soluciones del taller 8

## 1. Un grupo de orden 33 sólo tiene un $3$-subgrupo de Sylow.

Sea $S=\text{Syl}_3(G)$, por el tercer teorema de Sylow, $|S|$ divide a $33=3\cdot11$ y además, $|S|=3k+1$ para algún $k\in\mathbb{N}$. Por lo que o $|S|=1$, $|S|=3$ o $|S|=11$, necesariamente descartamos los últimos dos casos pues no existe $k$ natural que supla eso y por tanto $S=\{H\}$ donde $H$ es un $3$-subgrupo de Sylow y por tanto $H\unlhd G$, como cualquier otro $3$-subgrupo de Sylow es conjugado y $H$ es normal, sólo existe un grupo.

## 2. Sea $G$ un grupo de orden $p^r$ con $p$ primo. Entonces $G$ contiene un subgrupo normal de orden $p^{r-1}$.

Por el primer teorema de Sylow sabemos que existe $H\leq G$ con $|H|=p^{r-1}$, además sabemos que $H\unlhd N_G(H)$ y que $H\lneq N_G(H)$ donde $N_G(H)\leq G$. Por el teorema de Lagrange $|N_G(H)|=k$ donde $k|p^r$ y además sabemos que $r^{r-1}<k$ por lo que necesariamente $k=p^r$ y por tanto $G=N_G(H)$ luego $H\unlhd G$ y por el segundo teorema de Sylow, $H$ es único.

## 3. Sea $G$ un grupo finito. $G$ es simple si y sólo si $|G|$ es primo.

- ($\Rightarrow$): Falso.

- ($\Leftarrow$): Si el orden de $G$ es primo, entonces por el teorema de Lagrange, los únicos subgrupos de $G$ son él mismo y el trivial, por tanto es simple.

## 4. Ningún grupo de orden 15 es simple.

Como $15=1\cdot3\cdot5$, tomemos el conjunto $S$ de todos los $5$-subgrupos de Sylow de $G$, por el tercer teorema de Sylow $S=1$, o $S=3$ o $S=5$ y además $S=5k+1$ para algún natural $k$. Luego necesariamente $k=0$ y $S=\{H_5\}$ con $H_5\leq G$, así, dado que $gH_5g^{-1}\in S$ pues los conjugados de un $p$-grupo de Sylow también son un $p$-grupo de Sylow, necesariamente $gH_5g^{-1}=H_5$ para todo $g\in G$ y por tanto $H_5\unlhd G$. Luego $G$ no es simple.

## 5. Ningún grupo de orden $p^2q$ con $p$, $q$ primos distintos, es simple.

Sabemos que $\text{Syl}_p(G)|p^2q$ y además $\text{Syl}_p(G)=pk+1$ por lo que $\text{Syl}_p(G)\nmid p$ y por tanto hay 2 casos:

- Si $\text{Syl}_p(G)=1$, entonces el único $p$-subgrupo de Sylow es normal en $G$. 

- Si $\text{Syl}_p(G)=q$, entonces vamos a contar el número de elementos con orden $p^2$, dado que hay $q$ $p$-subgrupos de Sylow, hay $qp^2$ elementos con este orden, sin embargo estamos contando también a $e$ y por tanto existen $q(p^2-1)=p^2q-q$ elementos no neutros con orden $p^2$. 
  Ahora centrémonos en la cantidad de $q$-subgrupos de Sylow en $G$, similarmente tenemos que $\text{Syl}_q(G)\nmid q$ y $\text{Syl}_q(G)|p^2q$ por lo tanto hay 3 casos.
  
  - $\text{Syl}_q(G)=1$, entonces el único $q$-subgrupo de Sylow es normal en $G$.
  
  - $\text{Syl}_q(G)=p$, entonces tenemos que existen $p(q-1)$ elementos no neutros de orden $q$. Por lo tanto y añadiendo al neutro, tendríamos entre elemenos de orden $p$ y $q$
    
    $$
    \begin{align*}p^2q-q+pq-p+1&=p^2q+p(q-1)-(q-1)\\ &=p^2q+(p-1)(q-1)\end{align*}
    $$
    
    Como $p\neq q$ y por ser primos ambos son mayores o iguales a $2$, entonces $(p-1)(q-1)>1$ y por tanto concluimos que $|G|\lneq |G|$, lo que es una contradicción.
  
  - $\text{Syl}_q(G)=p^2$, dado que $1\lneq p$ entonces $p\lneq p^2$ y se sigue del argumento anterior que también se llega a una contradicción.
  
  Así, como cuando suponemos que si $\text{Syl}_p(G)\neq 1$ o $\text{Syl}_q(G)\neq 1$ llegamos a una contradicción, necesariamente alguno de los dos debe ser igual a 1 y por tanto debe existir un $z$-subgrupo normal en $G$ con $z$ primo.

En ambos casos llegamos a que existe un subgrupo normal $N$ tal que $\lang e\rang\lneq N\lneq G$ y por tanto $G$ no puede ser simple.

## 6. Ningún grupo de orden $20$ es simple.

Como $20=2^25$ y $2$ y $5$ son primos, los resultados del punto anterior demuestran que $G$ no es simple.

## 7. Todo grupo de orden $225$ es cíclico.

Como $225=3^25^2$, veamos que tanto sus $3$-subgrupos de Sylow como sus $5$-subgrupos de Sylow son normales. Por el tercer teorema de Sylow $|S_3(G)|$ y $|S_5(G)|$ (donde $S_p(G)$ es el conjunto de todos los $p$-subgrupos de Sylow de $G$), dividen a $225$ y tienen la forma $3k_1+1$ y $5k_2+1$ respectivamente, como $(5,3)=1$ y $3\neq2\neq5$ necesariamente ambos subgrupos son normales.
Por tanto $G=H_9\oplus H_{25}$, por otro lado, dado que $|H_9|=9=3^2$, $H_9$ es abeliano y análogamente con $H_{25}$. Concluimos que $G$ es abeliano.

## 8. Todo grupo de orden $p^2$ con $p$ primo, es abeliano.

Por el teorema de Cauchy sabemos que existe un elemento $x$ de orden $p$ en $G$ y además $\langle x\rangle\unlhd G$ pues $|x|=p^1$. Ahora, sea $G'=G/\lang x\rang$, $|G|=p$ y por tanto también tiene un elemento $y\lang x\rang$ con orden $p$. Por tanto, $G=\langle x,y\rangle$ donde $|x|=|y|=p$. Por lo que hay dos casos dada la definición de $y$, 

- Si $|yx|=p^2$ entonces $G\cong\mathbb{Z}_{p^2}$.

- Si $|yx|=p$ entonces $G\cong\mathbb{Z_p}\times\mathbb{Z_p}$.

En ambos casos concluimos $G$ es abeliano.

## 9. *Todo grupo simple de orden no primo, es de orden par.

>  No se hace.

## 10. Sea $G$ un grupo de orden $p^2q^2$, donde $p$ y $q$ son primos distintos tales que $q\nmid p^2-1$ y $p\nmid q^2-1$. Demuestre que $G$ es abeliano. Encuentre dos primos $p$ y $q$ para los cuales se cumpla esto.

## 11. Sea $G$ un grupo no abeliano de orden $p^3$ con $p$ primo. Entonces $|Z(G)|=p$.

Sabemos que $|Z(G)|=kp$ para algún $k\geq1$ y como $Z(G)\leq G$ entonces $kp|p^3$ y por tanto hay 3 opciones:

- $|Z(G)|=p$: La más chimba, queda demostrado lo que queríamos.

- $|Z(G)|=p^2$: Sabemos que $Z(G)\unlhd G$ y por tanto $|G/Z(G)|=p$, por lo que por el Teorema de Cauchy $G/Z(G)$ es cíclico y por tanto abeliano. Así, $G\cong Z(G)\times \mathbb{Z_p}$, que contradice que $G$ sea no abeliano.

- $|Z(G)|=p^3$: Entonces $Z(G)=G$, contradiciendo que $G$ es no abeliano.

## 12. Los únicos grupos de orden 99 son $\mathbb{Z_3\times Z_3\times Z_{11}}$ y $\mathbb{Z_9\times Z_{11}}$.

Sea $S$ el conjunto de los $3$-subgrupos de Sylow, como no existe $k\in\mathbb{N}$ tal que $11=3k+1$, entonces sólo existe un $3$-subgrupo de Sylow y es normal en $G$, análogamente llegamos a la misma conclusión con el $11$-subgrupo de Sylow, así, por teorema, $G=H_3\oplus H_{11}$, como $|H_3|=9$ sabemos que $H_3\cong\mathbb{Z_9}$ o $H_3\cong\mathbb{Z_3\times Z_3}$ , y como $|H_{11}|=11$ entonces $H_{11}\cong\mathbb{Z_{11}}$. Así o $G\cong\mathbb{Z_3\times Z_3\times Z_{11}}$ o bien $G\cong\mathbb{Z_9\times Z_{11}}$.

## 13. $A_4$ no es simple.

Sabemos que $|A_4|=\frac{4!}{2}=\frac{24}{2}=12=2^23$ , como $2$ y $3$ son primos, los resultados del punto $5$ garantizan que $A_4$ no es simple.

## 14. $A_5$ es simple.

Sabemos que $|A_5|=60=2^23^15^1$ 

## 15. Describa todos los subgrupos de Sylow de $S_4$.

## 16. Determine todos los grupos de orden 8.

## 17. Determine todos los grupos de orden 12.

## 18. Determine todos los grupos de orden 15 (salvo isomorfismo).

## 19. Determine todos los grupos de orden 10 (salvo isomorfismo).

## 20. Realice una tabla donde se vean todos los grupos de orden $n$ (salvo isomorfismo), para $n\leq15$.