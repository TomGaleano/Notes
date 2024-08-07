# Algunas soluciones de Taller 7

## 1. Sea $G=D_4=\{\rho_0,\rho_1,\rho_2,\rho_3,\mu_1,\mu_2,\delta_1,\delta_2\}$. Etiquete los vértices del cuadrado como $1,2,3,4$, los lados como $s_1,s_2,s_3,s_4$, las diagonales como $d_1,d_2$, los ejes vertical y horizontal como $m_1,m_2$, el centro del cuadrado como $C$ y los puntos medios de los lados como $P_1,P_2,P_3,P_4$ como se muestra en la figura.

![figura 16.9](https://hackmd.io/_uploads/ryi9MzrXA.png)

Sea $X=\{1,2,3,4,s_1,s_2,s_3,s_4,m_1,m_2,d_1,d_2,C,P_1,P_2,P_4\}$ y sea $\varphi$ una acción de $G$ en $X$ descrita en la siguiente tabla:

|            | $1$ | $2$ | $3$ | $4$ | $s_1$ | $s_2$ | $s_3$ | $s_4$ | $m_1$ | $m_2$ | $d_1$ | $d_2$ | $C$ | $P_1$ | $P_2$ | $P_3$ | $P_4$ |
| ---------- | --- | --- | --- | --- | ----- | ----- | ----- | ----- | ----- | ----- | ----- | ----- | --- | ----- | ----- | ----- | ----- |
| $\rho_0$   | $1$ | $2$ | $3$ | $4$ | $s_1$ | $s_2$ | $s_3$ | $s_4$ | $m_1$ | $m_2$ | $d_1$ | $d_2$ | $C$ | $P_1$ | $P_2$ | $P_3$ | $P_4$ |
| $\rho_1$   | $2$ | $3$ | $4$ | $1$ | $s_2$ | $s_3$ | $s_4$ | $s_1$ | $m_2$ | $m_1$ | $d_2$ | $d_1$ | $C$ | $P_2$ | $P_3$ | $P_4$ | $P_1$ |
| $\rho_2$   | $3$ | $4$ | $1$ | $2$ | $s_3$ | $s_4$ | $s_1$ | $s_2$ | $m_1$ | $m_2$ | $d_1$ | $d_2$ | $C$ | $P_3$ | $P_4$ | $P_1$ | $P_2$ |
| $\rho_3$   | $4$ | $1$ | $2$ | $3$ | $s_4$ | $s_1$ | $s_2$ | $s_3$ | $m_2$ | $m_1$ | $d_2$ | $d_1$ | $C$ | $P_4$ | $P_1$ | $P_2$ | $P_3$ |
| $\mu_1$    | $2$ | $1$ | $4$ | $3$ | $s_1$ | $s_4$ | $s_3$ | $s_2$ | $m_1$ | $m_2$ | $d_2$ | $d_1$ | $C$ | $P_1$ | $P_4$ | $P_3$ | $P_2$ |
| $\mu_2$    | $4$ | $3$ | $2$ | $1$ | $s_3$ | $s_2$ | $s_1$ | $s_4$ | $m_1$ | $m_2$ | $d_2$ | $d_1$ | $C$ | $P_3$ | $P_2$ | $P_1$ | $P_4$ |
| $\delta_1$ | $3$ | $2$ | $1$ | $4$ | $s_2$ | $s_1$ | $s_4$ | $s_3$ | $m_2$ | $m_1$ | $d_1$ | $d_2$ | $C$ | $P_2$ | $P_1$ | $P_4$ | $P_3$ |
| $\delta_2$ | $1$ | $4$ | $3$ | $2$ | $s_4$ | $s_3$ | $s_2$ | $s_1$ | $m_2$ | $m_1$ | $d_1$ | $d_2$ | $C$ | $P_4$ | $P_3$ | $P_2$ | $P_1$ |

1. Encuentre los conjuntos $X_\sigma$ para cada $\sigma\in G$:
   
   - $X_{\rho_0}=X$
   - $X_{\rho_1}=\{C\}$
   - $X_{\rho_2}=\{m_1,m_2,d_1,d_2,C\}$
   - $X_{\rho_3}=\{C\}$
   - $X_{\mu_1}=\{s_1,s_3,m_1,m_2,C,P_1,P_3\}$
   - $X_{\mu_2}=\{s_2,s_4,m_1,m_2,C,P_2,P_4\}$
   - $X_{\delta_1}=\{2,4,d_1,d_2,C\}$
   - $X_{\delta_2}=\{1,3,d_1,d_2,C\}$

2. Los grupos de isotropía $G_x$ para cada $x\in X$:
   
   - $G_{1}=\{\rho_0,\delta_2\}$
   - $G_{2}=\{\rho_0,\delta_1\}$
   - $G_{3}=\{\rho_0,\delta_2\}$
   - $G_{4}=\{\rho_0,\delta_1\}$
   - $G_{s_1}=\{\rho_0,\mu_1\}$
   - $G_{s_2}=\{\rho_0,\mu_2\}$
   - $G_{s_3}=\{\rho_0,\mu_1\}$
   - $G_{s_4}=\{\rho_0,\mu_2\}$
   - $G_{m_1}=\{\rho_0,\rho_2,\mu_1,\mu_2\}$
   - $G_{m_2}=\{\rho_0,\rho_2,\mu_1,\mu_2\}$
   - $G_{d_1}=\{\rho_0,\rho_2,\delta_1,\delta_2\}$
   - $G_{d_2}=\{\rho_0,\rho_2,\delta_1,\delta_2\}$
   - $G_C=G$
   - $G_{P_1}=\{\rho_0,\mu_1\}$
   - $G_{P_2}=\{\rho_0,\mu_2\}$
   - $G_{P_3}=\{\rho_0,\mu_1\}$
   - $G_{P_4}=\{\rho_0,\mu_2\}$

3. Las órbitas en $X$ bajo $D_4$
   
   - $\{1,2,3,4\}$
   
   - $\{s_1,s_2,s_3,s_4\}$
   
   - $\{m_1,m_2\}$
   
   - $\{d_1,d_2\}$
   
   - $\{C\}$
   
   - $\{P_1,P_2,P_3,P_4\}$
     
     ## 2. Sea $X$ un $G$-conjunto.

4. Muestre que para cada $g\in G$ la función $\sigma_g:X\to X$ deginida por $\sigma_g(x)=gx$ para cada $x\in X$ es una permutación en $X$.
   
    Partiendo de la definición, veamos que

$$
\begin{align*}\sigma_g:X&\to X\\ x&\mapsto gx\end{align*}
$$

Es una función biyectiva:

- **Inyectividad:** Sean $\sigma_g(x)=\sigma_g(y)$, esto es $gx=gy\in X$. Como $G$ es un grupo, $g^{-1}\in G$ y por tanto podemos usar $\sigma_{g^{-1}}:X\to X$ que sabemos es una función, por lo tanto tenemos que 

$$
\begin{align*} x&=\sigma_e(x)\\ &=\sigma_{g^{-1}g}(x)\\&=\sigma_{g^{-1}}(\sigma_g(x))\\&=\sigma_{g_{-1}}(\sigma_g(y))\\&=\sigma_{g^{-1}g}(y)\\&=\sigma_e(y)\\&=y\end{align*}
$$

- **Sobreyectividad:** Sea $z\in X$, como $\sigma_{g^{-1}}:X\to X$ es una función, $\sigma_{g^{-1}}(z)\in X$ y por tanto $\sigma_g(\sigma_{g^{-1}}(z))=z$.
2. Pruebe que la aplicacióñ definida por $\phi:G\to S_X$ definida por $\phi(g)=\sigma_g$ es un homomorfismo tal que $\phi(g)(x)=gx$  
   Sea $S_X$ el conjunto de todas las simetrías sobre $X$, veamos que $\phi$ define un homomorfismo:
- Sean $g_1,g_2\in G$,

$$
\begin{align*}\phi(g_1g_2)(x)&=\sigma_{g_1g_2}(x)\\&=\sigma_{g_1}(\sigma_{g_2}(x))\\&=\phi(g_1)\phi(g_2)(x)\end{align*}
$$

Ahora veamos que $\phi$ es un monomorfismo:

- Sean $g_1,g_2\in G$ tales que $\phi(g_1)=\phi(g_2)$, entonces $\sigma_{g_1}(x)=\sigma_{g_2}(x)$ para todo $x\in X$, esto es, $g_1x=g_2x$ para todo $x$ y por tanto, $g_2^{-1}(g_1(x))=g_2^{-1}(g_2(x))$ luego $g_2^{-1}g_1(x)=e(x)$ y por tanto $g_2^{-1}g_1=e$, es decir $g_1=g_2$.

## 3. Sea $H\leq G$, definimos $L_H$ como el conjunto de todas las clases laterales izquierdas de $H$. Muestre que $L_H$ es un $G$-conjunto

Definamos la función $\varphi$ dada por 

$$
\begin{align*}\varphi:G\times L_H&\to L_H\\(g,xH)&\mapsto (gx)H\end{align*}
$$

Veamos que $\varphi$ define una accióñ de $G$ sobre $L_H$:

- Sea $xH$ una clase lateral en $L_H$, sabemos que 

$$
\begin{align*}\varphi(e,xH)&=e(xH)\\&=(ex)H\\&=xH\end{align*}
$$

- Sean $g_1,g_2\in G$ y $xH\in L_H$, 

$$
\begin{align*}\varphi(g_1g_2,xH)&=(g_1g_2x)H\\&=g_1[(g_2x)H]\\&=g_1[\varphi(g_2,xH)]\\&=\varphi(g_1,\varphi(g_2,xH))\end{align*}
$$

Así, se suplen las dos condiciones para que $\varphi$ represente una acción y por tanto $L_H$ es un $G$-conjunto.

## 4. Calcule todas las acciones del grupo $\mathbb{Z_3}$ sobre el conjunto $\mathbb{Z_2}$

- La acción trivial $\varphi_0$ tal que $\varphi_0(m,n)=n$, $\forall m\in\mathbb{Z_3}$, $\forall n\in\mathbb{Z_2}$.
- La acción definida por 

$$
\begin{align*}\varphi:\mathbb{Z}_3\times \mathbb{Z}_2 &\to \mathbb{Z}_2\\ (\overline{n},\overline{m})&\mapsto \overline{n+m}\end{align*}
$$

Usando la asociatividad de la suma en $\mathbb{Z_2}$ y que el $\overline{0}$ es neutro en ambos grupos.

> Aquí no supe sacar más acciones de manera intuitiva.

### Análisis más profundo:

Intentando asignar manualmente una imágen a cada elemento, primero comprendiendo a $\mathbb{Z_3}:=\{a:a^3=e\}$  y a $\mathbb{Z_2}:=\{a':(a')^2=e'\}$ vemos que es de la forma:

$$
\begin{align*}\varphi:\mathbb{Z_3\times Z_2}&\to\mathbb{\Z_2}\\(e,e')&\mapsto e'\\ (e,a')&\mapsto a'\\(a,e')&\mapsto ae'\\(a,a')&\mapsto aa'\\(a^2,e')&\mapsto a^2e'\\(a^2, a')&\mapsto a^2a'\end{align*}
$$

Dado que estamos trabajando con acciones y un grupo cíclico abeliano, sabemos que $\varphi(a^{n+1},x)=\varphi(a\cdot a^n, x)=\varphi(a,\varphi(a^n,x))$ por lo que podemos definir las acciones de forma recursiva, así, sólo tenemos que definir $ae'$ y $aa'$, usando que $|\mathbb{Z_2}|=2$ y que tanto $ae'$ como $aa'$ deben ser elementos de este, podemos definir cuatro acciones $\varphi_i$ distintas:

- $\varphi_0:$ Si $ae'=e'$ y $aa'=a'$, entonces $a^2e'=a(ae')=a(e')=e'$ y análogamente $a^2a'=a'$, por lo que $\varphi_0$ representa la acción trivial.

- $\varphi_1:$ Si $ae'=a'$ y $aa'=e'$, entonces $a^2e'=a(ae')=a(a')=e'$ y análogamente $a^2a'=a'$, por lo que $\varphi_1$ coincide con la segunda acción que definimos arriba.
  
  > Aquí asumo que puede darse que $aa'$ puede ser igual a $ae'$, por lo que ví sigue siendo acción.

- $\varphi_2:$ Si $ae'=e'=aa'$ entonces $a^2e'=a(ae')=ae'=e'=aa'=a^2a'$.

- $\varphi_3:$ Si $ae'=a'=aa'$ entonces $a^2e'=a(ae')=aa'=a'=ae'=a^2a'$.
  
  > ¿Son las únicas? Como lo veo si en lugar de definir $ae'$ y $aa'$ defino $a^2e'$ y $a^2a'$ como $(a^2)^2=a$ entonces necesariamente debo usarlos para definir $ae'$ y $aa'$. Entonces no conozco otra forma de construir una acción diferente.

## ¿Teorema?

### Sean $\mathbb{Z_m}$ y $\mathbb{Z_n}$ con $(m,n)=1$ y $\Phi:=\{\varphi:\mathbb{Z_m\times Z_n}\to\mathbb{Z_n}\ |\ \varphi\text{ es una acción}\}$, entonces $|\Phi|=|S_n|=n!$

> No me cuadra ese $(m,n)=1$. Lo importante es hacer que $\alpha^m=e$ para todo $\alpha\in S_n$. ¿Cómo?

Planteemos la función 

$$
\begin{align*}
f:S_n&\to\Phi\\
\alpha&\mapsto \varphi_\alpha
\end{align*}
$$

Donde

$$
\begin{align*}\varphi_\alpha:\mathbb{Z_m\times Z_n}&\to\mathbb{Z_n}\\ (m,n)&\mapsto \alpha^m(n)\end{align*}
$$

##### Primero, veamos que efectivamente $\varphi_\alpha\in\Phi$.

- $\varphi_\alpha(0,n)=\alpha^0(n)=I(n)=n$, $\forall n\in\mathbb{Z_n}$.

- $\varphi_\alpha(m_1+m_2,n)=\alpha^{m_1+m_2}(n)=\alpha^{m_1}(\alpha^{m_2}(n))=\varphi_\alpha(m_1,\varphi_\alpha(m_2,n)).$

Además, dado que $\mathbb{Z_m}$ es finito y cíclico, necesitamos que si $m_1+m_2\equiv_m0$, entonces $\varphi_\alpha(m_1+m_2,n)=\varphi_\alpha(0,n)$. Como $(m,n)=1$ y $m_1+m_2=km$ con $k\in\mathbb{N}$, entonces $\alpha^{m_1+m_2}(n)=\alpha^{km}(n)=(\alpha^m)^k(n)=I^k(n)=I (n)=\varphi_\alpha(0,n)$.

##### Ahora, veamos que $f$ es inyectiva:

Sean $\alpha,\beta\in S_n$ tales que $f(\alpha)=f(\beta)$, entonces $\varphi_\alpha(m,n)=\varphi_\beta(m,n)$ para todos $m\in\mathbb{Z_m}$ y $n\in\mathbb{Z_n}$, particularmente $\varphi_\alpha(1,n)=\varphi_\beta(1,n)$, esto es, $\alpha(n)=\beta(n)$ para todo $n\in\mathbb{Z_n}$ por lo que concluimos $\alpha=\beta$.

##### Por último, veamos que $f$ es sobreyectiva:

Sea una acción $\varphi_x\in\Phi$, sabemos que $\varphi_x(1,n)\in\mathbb{Z_n}$ para todo $n\in\mathbb{Z_n}$. Así, definimos $y\in S_n$ dado por

$$
\begin{align*}y:N&\to N\\k&\mapsto\varphi_x(1,k)\end{align*}
$$

Donde $N=\{0,1,...,n-1\}$.

Veamos que $f(y)=\varphi_x$:

Por la construcción misma, sabemos que $\varphi_y(1,k)=y^1(k)=y(k)=\varphi_x(1,k)$, y como $\lang1\rang=\mathbb{Z_m}$, el resto de imágenes coinciden naturalmente, finalmente usando que $(m,n)=1$, tenemos que $\varphi_y(m,k)=y^m(k)$