# Tarea Acciones de Grupo

###### Maira Florez y Tomás Galeano

## Sea $X$ un $G$-conjunto:

### a). Muestre que para cada $g\in G$ la función $\sigma_g:X\to X$ definida por $\sigma_g(x)=gx$ para $x\in X$ es una permutación en $X$.

Recordando que por definición, 

> Una permutación de un conjunto $A$ es una función biyectiva $\phi:A\to A$.

Por otro lado, si $X$ es un $G$-conjunto es porque existe una función

$$
\begin{align*}
\varphi:G\times X&\to X\\ 
(g,x)&\mapsto gx
\end{align*}
$$

Que además cumple que

1. $ex=x$, $\forall x\in X$.

2. $(g_1g_2)x=g_1(g_2x)$, $\forall g_1,g_2\in G$ y $\forall x\in X$.

Tenemos que comprobar que $\sigma_g$ es biyectivo para todo $g\in G$.

- **Inyectividad:** Sean $x,y\in X$ tales que $\sigma_g(x)=\sigma_g(y)$ para algún $g\in G$. Sabemos que $G$ es un grupo por lo que $g^{-1}\in G$ y así $\sigma_{g^{-1}}$ es también una función bien definida. Evaluando $\sigma_g(x)$ en $\sigma_{g^{-1}}$ tenemos que
  
  $$
  \begin{align*}
x&=ex\\
&=(g^{-1}g)x\\
&=g^{-1}(gx)\\
&=\sigma_{g^{-1}}(\sigma_g(x))\\
&=\sigma_{g^{-1}}(\sigma_g(y))\\
&=g^{-1}(gy)\\
&=(g^{-1}g)y\\
&=ey\\
&=y
\end{align*}
  $$
  
  Y por tanto $x=y$.

- **Sobreyectividad:** Sea un elemento $z\in X$, nuevamente usando la existencia y buena fundación de $\sigma_{g^{-1}}$ para todo $g\in G$, sabemos que $\sigma_{g^{-1}}(z)\in G$, así, y usando la definición de $\sigma_g$, tenemos que
  
  $$
  \begin{align*}
\sigma_g(\sigma_{g^{-1}}(z))&=\sigma_g(g^{-1}z)\\
&=g(g^{-1}z)\\
&=(gg^{-1})z\\
&=ez\\
&=z
\end{align*}
  $$
  
  Así, tenemos que para todo elemento de $X$ existe una preimagen por $\sigma_g$.

Por estos dos puntos, $\sigma_g$ es una biyección sobre $X$ para todo $g\in G$ y por tanto una permutación.

### b). Pruebe que la aplicación definida por $\phi: G\to S_X$ definida por $\phi(g)=\sigma_g$ es un homomorfismo tal que $\phi(g)(x)=\sigma_g(x)$ para todo $x\in X$.

Sean $g_1$ y $g_2$ en $G$, veamos que $\phi(g_1\cdot g_2)=\phi(g_1)\circ\phi(g_2)$. Para esto, debemos ver que $\sigma_{g_1\cdot g_2}(x)=(\sigma_{g_1}\circ \sigma_{g_2})(x)$, para todo $x\in X$. Tenemos que:

$$
\begin{align*}
\sigma_{g_1\cdot g_2}(x)&=(g_1\cdot g_2)(x)\\
&=g_1(g_2x)\\
&=g_1(\sigma_{g_2}(x)\\
&=\sigma_{g_1}(\sigma_{g_2}(x))\\
&=(\sigma_{g_1}\circ\sigma_{g_2})(x)
\end{align*}
$$

Por tanto $\phi$ es un homomorfismo.
