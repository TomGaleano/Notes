# Tarea Suma Directa Interna

###### Maira Florez y Tomás Galeano

## 1. ¿Puede escribir $D_4$ como la suma directa interna de dos de sus subgrupos? Explique.

Sea $D_4=\lang f,r:f^2=r^4=e,\ rfr=f^{-1}\rang$, sabemos que sus subgrupos normales son:

- $N_0=\{e\}$

- $N_1=\lang r^2\rang$

- $N_2=\lang r\rang$

- $N_3=\{e,rf,r^2,fr\}$

- $N_4=D_4$

Así, vemos que para todos subgrupos normales $H$, $K\unlhd D_4$, si $H\neq N_0\neq K$ entonces $H\cap K\neq\{e\}$ por lo que para describir $D_4$ como suma directa de dos de sus subgrupos, necesitamos que al menos uno de ellos sea $N_0$. Así, lógicamente el otro subgrupo debe ser $D_4$ mismo y por tanto la única opción es

$$
D_4=N_0\oplus N_4
$$

## 2. Encuentre todas las descomposiciones de $S_3$ como suma directa de dos de sus subgrupos.

Dado que $S_3\cong D_3$, entonces trabajaremos con la definición de $D_3=\lang f,r:f^2=r^3=e,rfr=f^{-1}\rang$, así, sus subgrupos normales son:

- $N_0=\{e\}$

- $N_1=\lang r\rang$

- $N_2=D_3$

Teniendo en cuenta que como $N_0N_1\neq D_3$ y $N_1\cap N_2\neq\{e\}$, entonces la única opción es que

$$
D_3=N_0\oplus N_2
$$
