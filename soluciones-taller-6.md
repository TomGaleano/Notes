# Soluciones del taller 6
## 1. Haga una lista de todos los elementos de $\mathbb{Z_3\times Z_4}$.
- $(0,0)$
- $(1,0)$
- $(2,0)$
- $(0,1)$
- $(0,2)$
- $(0,3)$
- $(1,1)$
- $(1,2)$
- $(1,3)$
- $(2,1)$
- $(2,2)$
- $(2,3)$
## 2. Encuentre generadores para cada uno de los siguientes grupos
1. $\mathbb{Z\times Z_2}:\{(1,0),(0,1)\}$
2. $\mathbb{Z_2\times Z_3}:\{(1,1)\}$
3. $\mathbb{Z_4\times Z_5}:\{(1,1)\}$
## 3. Encuentre el orden de $(3,4,8)$ en $\mathbb{Z_6\times Z_{12}\times Z_{24}}$.
$\text{ord(3,4,8)}=\text{m.c.d}(\text{ord}(3),\text{ord}(4),\text{ord}(8))=\text{m.c.d}(2,3,3)=6$.
## 4. Determine el mayor orden posible para un elemento de $\mathbb{Z_4\times Z_6}$.
Individualmente, el mayor orden de un elemento en $\mathbb{Z_4}$ es $4,\ (1,3)$ mientras que en $\mathbb{Z_6}$ es $6,\ (1,5)$. Así, el mayor orden en $\mathbb{Z_4\times Z_6}$ es $\text{m.c.d}(4,6)=12$.
## 5. ¿Es $\mathbb{Z_2\times\mathbb{Z_4}}$ isomorfo a $\mathbb{Z_8}$?
No. Por teorema se tiene que $\mathbb{Z_p\times Z_q\cong Z_{pq}}$ si y solo si $\text{m.c.d}(p,q)=1$.
## 6. Sea $V$ el cuarto grupo de Klein ¿Podemos decir que $V\cong\mathbb{Z_2\oplus Z_2}$?
Dado que $\mathbb{Z_2\cap Z_2\neq\{0\}}$, no podemos usar la suma directa interna, luego analizamos la suma directa externa que para una familia de grupos finita coincide con el producto directo, así, definimos:
$$\begin{align*}\varphi:V&\to\mathbb{Z_2\times Z_2}\\ e&\mapsto (0,0)\\ a&\mapsto(1,0) \\ b&\mapsto(0,1) \\ ab&\mapsto(1,1)\end{align*}$$
Que puede demostrarse por extensión (caso por caso), es un isomorfismo.
## 7. ¿Qué se puede decir de $\mathbb{Z_m\times Z_n}$ cuando $m$ y $n$ son primos relativos?
Que el producto es isomorfo a $\mathbb{Z_{mn}}$ y $\mathbb{Z_m\times Z_n}=\langle(1,1)\rangle$.
## 8. Sea $G=G_1\times G_2$ el producto directo de los grupos $G_1,G_2$. Determine el centro de $G$.
Veamos que $Z(G)=Z(G_1)\times Z(G_2)$:
- $Z(G)\subseteq Z(G_1)\times Z(G_2):$ Sea $x\in Z(G)$, $xy=yx$, $\forall y\in G$, donde $x=(x_1,x_2)$ y $y=(y_1,y_2)$ y por la forma en la que esta definida el producto directo se tiene que $x_1y_1=y_1x_1$ para todo $y_1\in G_1$, por lo que $x_1\in Z(G_1)$ y análogamente $x_2\in Z(G_2)$, así, $(x_1,x_2)=x\in Z(G_1)\times Z(G_2)$.
- $Z(G)\supseteq Z(G_1)\times Z(G_2):$ Sean $x\in G_1$, $y\in G_2$, naturalmente $(x,y)\in G_1\times G_2$, ahora, sea $(a,b)\in G$ donde $a\in G_1$ y $b\in G_2$, se tiene que por la definición de producto directo, $$(x,y)(a,b)=(xa,yb)=(ax,by)=(a,b)(x,y)$$
Así, $(x,y)\in Z(G)$ y por la doble contenencia, queda demostrado que $Z(G)=Z(G_1)\times Z(G_2)$.
## 9. Sea $G=A_1\times A_2\times ...\times A_n$ y suponga que $B_i$ es un subgrupo normal de $A_i$ para cada $i=1,2,...,n$. Pruebe que $B_1\times B_2\times ...\times B_n$ es normal en $G$ y que $$(A_1\times A_2\times...\times A_n)/(B_1\times B_2\times ...\times B_n)\cong (A_1/B_1)\times(A_2/B_2)\times...\times (A_n/B_n)$$
Para simplificar notación definimos $I=\{1,2,...,n\}$, $B=\prod_{i\in I}B_i$ y $A=\prod_{i\in I}A_i$.
Veamos primero que $B\leq A$. Dado que $B_i\leq A_i$ para todo $i$, se tiene que $e_i\in B_i$ y por tanto, $(e_1,e_2,...,e_n)\in B$ luego $B\neq\varnothing$.
Ahora, sean $x=(x_1,x_2,...,x_n)$ y $y=(y_1,y_2,...,y_n)$ en $B$, se tiene que $x_i,y_i\in B_i$ con $i\in I$, como $B_i\leq A_i$ se tiene que $y^{-1}_i\in B_i$ y además $x_iy^{-1}_i\in B_i$ por lo que $(x_1y_1^{-1}, x_2y_2^{-1},...,x_ny_n^{-1})=xy^{-1}\in B$. Así $B\leq A$. 
Ahora veamos que $B\unlhd A$ probando que $yxy^{-1}\in B$ para todo $x\in B$ y $y\in A$:
Sea $x\in B$, $x=(x_1,x_2,...,x_n)$, y sea un elemento cualquiera $y\in A$, $y=(y_1,y_2,...,y_n)$ sabemos que$$yxy^{-1}=(y_1,y_2,...,y_n)(x_1,x_2,...,x_n)(y_1^{-1},y_2^{-1},...,y^{-1}_n)=(y_1x_1y^{-1}_1,y_2x_2y^{-1}_2,...,y_nx_ny^{-1}_n)$$
Como $A_i$ es normal para todo $i$, $y_ix_iy_i^{-1}\in A_i$ para todos $y_i\in A_i$, $x_i\in A_i$ e $i\in I$. Por tanto $yxy^{-1}\in B$ y concluimos que es normal con respecto a $A$. Así, podemos hacer la partición $A/B$ y definir la siguiente función:
$$\begin{align*}\varphi:A/B&\to\prod_{i\in I}A_i/B_i\\ [f]=\{f_b\}_{b\in B}&\mapsto (\{f_b(i)\}_{b\in B})_{i\in I}\end{align*}$$Donde usamos hecho que la clase de un elemento $f\in A$ es $[f]=\{fb:b\in B\}$ y por tanto, un elemento $x\in A/B$ es una familia de funciones con dominio $I$. Ahora, veamos que esta función está bien definida:
Sean $f,g\in [f]$, sabemos que $g=f_{b_j}$ para algún $b_j\in B$ y $j\in |B|$, así, $$\begin{align*}\varphi([g])&=(\{g_{b_1}(1),g_{b_2}(1),...,g_{b_{k_1}}(1)\},...,\{g_{b_1}(n),g_{b_2}(n),...,g_{b_{k_n}}(n)\})\\ &=(\{f_{b_jb_1}(1),f_{b_jb_2}(1),...,f_{b_jb_{k_1}}(1)\},...,\{f_{b_jb_1}(n),f_{b_jb_2}(n),...,f_{b_jb_{k_n}}(n)\})\\ &= (\{f_{b'_1}(1),f_{b'_2}(1),...,f_{b'_{k_1}}(1)\},...,\{f_{b'_1}(n), f_{b'_2}(n),..., f_{b'_{k_n}}(n)\})\\ &=\varphi([f])\end{align*}$$
usando el hecho que $B_i$ es cerrado pues es un subgrupo y también definimos $k_i=|B_i|$ para $i\in I$.
Veamos que $\varphi$ es un homomorfismo: sean $[x],[y]\in A/B$,$$\begin{align*}\varphi([x][y])&=\varphi(\{x_{b_1}y_{b_2}\}_{b_1,b_2\in B})\\ &=(\{x_{b_1}y_{b_2}(i)\}_{b_1,b_2\in B})_{i\in I}\\ &=(\{x_{b_1}(i)\}_{b_1\in B})_{i\in I}(\{y_{b_2}(i)\}_{b_2\in B})_{i\in I}\\ &=\varphi([x])\varphi([y])\end{align*}$$
Si $\varphi([x])=\varphi([y])$ entonces $(\{x_b(i)\}_{b\in B})_{i\in I}=(\{y_{b'}(i)\}_{b'\in B})_{i\in I}$ entonces son iguales componente a componente, luego $x(i)\in\{y_{b'}(i)\}_{b\in B}$ por lo que $x\in [y]$, así, necesariamente $[x]=[y]$ y concluimos $\varphi$ es un monomorfismo.

Ahora, sea $x\in \prod_{i\in I}A_i/B_i$, $x=([a_1],[a_2],...,[a_n])$ entonces podemos definir $f\in A$ tal que $f(i)=a_i$, $\forall i\in I$. Naturalmente $f\in[f]$ y además se tiene que $\varphi([f])=(\{f_b(i)\}_{b\in B})_{i\in I}$, particularmente $e\in B$ por lo que $a_i\in\{f_b(i)\}_{b\in B}$ y por tanto $[a_i]=\{f_b(i)\}_{b\in B}$ por lo que $\varphi([f])=x$. Concluimos que $\varphi$ es además un epimorfismo.

Así, $\varphi$ resulta un isomorfismo.
## 10. Verifique que $\mathbb{C=R\oplus iR}$.
Se asume que la operación en $\mathbb{C}$ es la suma usual que es conmutativa, por la definición de la suma componente a componente en los complejos, inmediatamente $\mathbb{R\leq C}$ e $\mathbb{iR\leq C}$, además, dado que los complejos son abelianos, se tiene que $\mathbb{R,iR\unlhd C}$. Por último sabemos que $\mathbb{C=R(iR)}$ y que $\mathbb{R\cap iR=\{0\}}$, así, por teorema tenemos que $\mathbb{C=R\oplus iR}$.
## 11. Escriba el cuarto grupo de Klein como suma directa interna de dos de sus subgrupos. Explique
Dado que $V$ es abeliano, todos sus subgrupos son normales, a su vez, $e=e\cdot e$, $a=a\cdot e$, $b=e\cdot b$ y $ab=a\cdot b$ por lo que $V=\langle a\rangle\langle b\rangle$. Así y dado que $\langle a\rangle\cap\langle b\rangle=\{e\}$, se tiene que $V=\langle a\rangle \oplus\langle b\rangle$.
## 12. ¿Puede escribir $D_4$ como la suma directa interna de dos de sus subgrupos? Explique.
Claro, sea $\langle f\rangle$ el subgrupo de rotaciones en $D_4$, sabemos que $|\langle f\rangle|=4$, por otro lado sea $\langle g\rangle$ el subgrupo de las reflexiones, donde $|\langle g\rangle|=2$. Se tiene que $|\langle f\rangle \times \langle g\rangle|=|D_4|=8$, además, $\langle f\rangle\cap\langle g\rangle=\{e\}$, por último, se tiene que todo elemento $x$ de $D_4$ se puede descomponer en terminos de potencias de reflexiones y de rotaciones. Por tanto $D_4=\langle f\rangle\oplus\langle g\rangle$. 
## 13. Sea $G$ un grupo, $M$, $N$ subgrupos de $G$ y $M\unlhd G$. Suponga además que $M\cap N=\{e\}$ y $G=MN$. Pruebe que $G$ es isomorfo al producto semi-directo de $M$ y $N$.
Planteamos la acción de grupo de $N$ en $M$ dada por:$$\begin{align*}\varphi:N\times M&\to M\\ (n,m)&\mapsto nmn^{-1}\end{align*}$$
Haciendo uso de que $M$ es normal, podemos entonces definir el producto en $M \rtimes N$ donde para $m_1,m_2\in M$ y $n_1,n_2\in N$,$$(m_1,n_1)(m_2,n_2)=(m_1\varphi_{n_1}(m_2),n_1n_2)=(m_1n_1m_2n_1^{-1},n_1n_2)$$
Así, definimos el homomorfismo$$\begin{align*}\phi:M\rtimes N&\to G\\ (m,n)&\mapsto mn\end{align*}$$
Veamos que $\phi$ es un homomorfismo, sean $(x_1,y_1)(x_2,y_2)\in M \rtimes N$:$$\begin{align*}\phi[(x_1,y_1)(x_2,y_2)]&=\phi[x_1y_1x_2y_1^{-1},y_1y_2]\\ &= x_1y_1x_2y_1^{-1}y_1y_2 \\ &=x_1y_1x_2y_2 \\ &= \phi[(x_1,y_1)]\phi[(x_2,y_2)]\end{align*}$$
Por último, como sabemos que $G=MN$,sabemos que $\phi$ es un isomorfismo y por tanto $G\cong M\rtimes N$.
## 14. Encuentre todas las descomposiciones de $S_3$ como suma directa de dos de sus subgrupos.
Sea $S_3=\{\rho_0,\rho_1,\rho_2,r_1,r_2,r_3\}$, solo se cuenta con un subgrupo de 3 elementos, $\langle \rho_1 \rangle$ y 3 subgrupos de 2 elementos $\langle r_i\rangle$ con $1\leq i\leq3$. Así,
$$S_3=\langle\rho_1\rangle\oplus\langle r_1\rangle=\langle\rho_1\rangle\oplus\langle r_2\rangle=\langle\rho_1\rangle\oplus\langle r_3\rangle$$