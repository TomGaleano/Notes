# Tarea Producto de Grupos

###### Maira Florez y Tomás Galeano

## 1. Sea $G=G_1\times G_2$, el producto directo de los grupos $G_1$ y $G_2$. Determinar el centro de $G$.

Veamos que $Z(G)=Z(G_1)\times Z(G_2):$

- $Z(G)\subseteq Z(G_1)\times Z(G_2)$: Sea $x\in Z(G), xy=yx$, $\forall y\in G$, donde $x=(x_1,x_2)$ y $y=(y_1,y_2)$. Por la forma en la que esta definida el producto directo se tiene que $x_1y_1=y_1x_1$ para todo $y_1\in G_1$, por lo que $x_1\in Z(G_1)$ y análogamente $x_2\in Z(G_2)$, así, $(x_1,x_2)=x\in Z(G_1)\times Z(G_2)$.

- $Z(G)\supseteq Z(G_1)\times Z(G_2)$: Sean $x\in Z(G_1)$, $y\in Z(G_2)$, naturalmente y dado que $Z(G_i)\leq G_i$ para $i\in\{1,2\}$, entonces $(x,y)\in  G_1\times G_2$, ahora, sea $(a,b)\in G$ donde $a\in G_1$ y $b\in G_2$, se tiene que por la definición de producto directo, $(x,y)(a,b)=(xa,yb)=(ax,by)=(a,b)(x,y)$.
  
  Así, $(x,y)\in Z(G)$ y por la doble contenencia, queda demostrado que $Z(G)=Z(G_1)\times Z(G_2)$.

## 2. Sea $G=A_1\times A_2\times ...\times A_n$ y suponga que $B_i$ es un subgrupo normal de $A_i$ para cada $i=1,2,...,n$. Pruebe que $B_1\times B_2\times ...\times B_n$ es normal en $G$ y que

$$
(A_1\times A_2\times...\times A_n)/(B_1\times B_2\times ...\times B_n)\cong (A_1/B_1)\times(A_2/B_2)\times...\times (A_n/B_n)
$$

Para simplificar notación definimos $I=\{1,2,...,n\}$,a $B=\prod_{i\in I}B_i$ y $A=\prod_{i\in I}A_i$.

- Veamos primero que $B\leq A$. 
  
  Dado que $B_i\leq A_i$ para todo $i$, se tiene que $e_i\in B_i$ y por tanto, $(e_1,e_2,...,e_n)\in B$ luego $B\neq\varnothing$.
  Ahora, sean $x=(x_1,x_2,...,x_n)$ y $y=(y_1,y_2,...,y_n)$ en $B$, se tiene que $x_i,y_i\in B_i$ con $i\in I$, como $B_i\leq A_i$ se tiene que $y^{-1}_i\in B_i$ y además $x_iy^{-1}_i\in B_i$ por lo que $(x_1y_1^{-1}, x_2y_2^{-1},...,x_ny_n^{-1})=xy^{-1}\in B$. Concluyendo que $B\leq A$. 

- Ahora veamos que $B\unlhd A$ probando que $yxy^{-1}\in B$ para todo $x\in B$ y $y\in A$:
  Sea $x\in B$, $x=(x_1,x_2,...,x_n)$, y sea un elemento cualquiera $y\in A$, $y=(y_1,y_2,...,y_n)$ sabemos que
  
  $$
  \begin{align*}
yxy^{-1}&=(y_1,y_2,...,y_n)(x_1,x_2,...,x_n)(y_1^{-1},y_2^{-1},...,y^{-1}_n)
\\&=(y_1x_1y^{-1}_1,y_2x_2y^{-1}_2,...,y_nx_ny^{-1}_n)
\end{align*}
  $$
  
  Como $B_i\unlhd A_i$ , $y_ix_iy_i^{-1}\in B_i$ para todos $y_i\in A_i$, $x_i\in B_i$ e $i\in I$. Por tanto $yxy^{-1}\in B$ y concluimos que es normal con respecto a $A$.

##### Ahora bien hay dos formas de probar el isomorfismo de los cocientes:

1. Demos la siguiente función $\varphi$:
   
   $$
   \begin{align*}\varphi:A/B&\to\prod_{i\in I}A_i/B_i\\ [f]=\{f_b\}_{b\in B}&\mapsto (\{f_b(i)\}_{b\in B})_{i\in I}\end{align*}
   $$
   
   Donde usamos hecho que la clase de un elemento $f\in A$ es $[f]=\{fb:b\in B\}$ y por tanto, un elemento $x\in A/B$ es una familia de funciones con dominio $I$. Ahora, veamos que nuestra función $\varphi$ está **bien definida**:
   Sean $f,g\in [f]$, sabemos que $g=f_{b_j}$ para algún $b_j\in B$ y $j\in |B|$, así,
   
   $$
   \begin{align*}\varphi([g])&=(\{g_{b_1}(1),g_{b_2}(1),...,g_{b_{k_1}}(1)\},...,\{g_{b_1}(n),g_{b_2}(n),...,g_{b_{k_n}}(n)\})\\ &=(\{f_{b_jb_1}(1),f_{b_jb_2}(1),...,f_{b_jb_{k_1}}(1)\},...,\{f_{b_jb_1}(n),f_{b_jb_2}(n),...,f_{b_jb_{k_n}}(n)\})\\ &= (\{f_{b'_1}(1),f_{b'_2}(1),...,f_{b'_{k_1}}(1)\},...,\{f_{b'_1}(n), f_{b'_2}(n),..., f_{b'_{k_n}}(n)\})\\ &=\varphi([f])\end{align*}
   $$
   
   usando el hecho que $B_i$ es cerrado pues es un subgrupo y también definimos $k_i\in|B_i|$ para $i\in I$.
   Veamos que $\varphi$ es un **homomorfismo**: sean $[x],[y]\in A/B$,
   
   $$
   \begin{align*}\varphi([x][y])&=\varphi(\{x_{b_1}y_{b_2}\}_{b_1,b_2\in B})\\ &=(\{x_{b_1}y_{b_2}(i)\}_{b_1,b_2\in B})_{i\in I}\\ &=(\{x_{b_1}(i)\}_{b_1\in B})_{i\in I}(\{y_{b_2}(i)\}_{b_2\in B})_{i\in I}\\ &=\varphi([x])\varphi([y])\end{align*}
   $$
   
   Si $\varphi([x])=\varphi([y])$ entonces $(\{x_b(i)\}_{b\in B})_{i\in I}=(\{y_{b'}(i)\}_{b'\in B})_{i\in I}$ entonces son iguales componente a componente, luego $x(i)\in\{y_{b'}(i)\}_{b\in B}$ por lo que $x\in [y]$, así, necesariamente $[x]=[y]$ y concluimos $\varphi$ es un **monomorfismo**.
   
   Ahora, sea $x\in \prod_{i\in I}A_i/B_i, x=([a_1],[a_2],...,[a_n])$ entonces podemos definir $f\in A$ tal que $f(i)=a_i, \forall i\in I$. Naturalmente$ f\in[f]$ y además se tiene que $\varphi([f])=(\{f_b(i)\}_{b\in B})_{i\in I}$, particularmente $e\in B$ por lo que $a_i\in\{f_b(i)\}_{b\in B}$ y por tanto $[a_i]=\{f_b(i)\}_{b\in B}$ por lo que $\varphi([f])=x$. Concluimos que $\varphi$ es además un **epimorfismo**.
   
   Así, $\varphi$ resulta un **isomorfismo**.

2. Definamos otra función
   
   $$
   \begin{align*}
\phi:A&\to\prod_{i\in I}A_i/B_i\\
(a_i)_{i\in I}&\mapsto([a_i])_{i\in I}
\end{align*}
   $$
   
   Veamos que $\phi$ es un **homomorfismo**:
   
   Sean $(x_i)_{i\in I}$, $(y_i)_{i\in I}\in A$, tenemos que
   
   $$
   \begin{align*}
\phi((x_i)_{i\in I}\cdot(y_i)_{i\in I})&=\phi((x_iy_i)_{i\in I})\\
&=([x_iy_i])_{i\in I}\\
&=(B_ix_iy_i)_{i\in I}\\
&=(B_ix_i)_{i\in I}(B_iy_i)_{i\in I}\\
&=([x_i])_{i\in I}([y_i])_{i\in I}\\
&=\phi((x_i)_{i\in I})\phi((y_i)_{i\in I})
\end{align*}
   $$
   
   Donde usamos que $([a_i])_{i\in I}=(B_ia_i)_{i\in I}$ para todo $a\in A$.
   
   Ahora, probemos que $\text{ker}(\phi)=B$.
   
   Sea $x\in\text{ker}(\phi)$,
   
   $$
   \begin{align*}
x\in\text{ker}(\phi)&\Leftrightarrow \phi(x)=([e_i])_{i\in I}\\
&\Leftrightarrow \phi(x)=(B_i)_{i\in I}\\
&\Leftrightarrow x(i)\in B_i,\ \forall i\in I\\
&\Leftrightarrow x\in B
\end{align*}
   $$
   
   Por último, veamos que $\phi$ es sobreyectiva:
   
   Sea $y\in\prod_{i\in I}A_i/B_i$, $y$ es una $n$-upla donde cada componente es una clase lateral de $A_i/B_i$, así, $y=([x_i])_{i\in I}$ donde $x_i\in A_i$, por lo que podemos formar la preimagen $x=(x_1,x_2,...,x_n)\in A$ y es natural que $\phi(x)=y$. Por lo que concluimos que $\phi$ es un **epimorfismo**.
   
   Así, por el **Teorema Fundamental del Homomorfismo**, tenemos que

$$
A/B\cong \prod_{i\in I}A_i/B_i
$$

    Quedando por ambos caminos demostrado lo que buscabamos.
