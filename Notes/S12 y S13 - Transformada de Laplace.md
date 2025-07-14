---
tags:
  - Math/EDO
date / time: 2025-06-13T12:16:00
Status: false
---
> [!abstract] Abstract
> Contents

---
# Transformadas de Laplace
## Tabla de transformadas de Laplace
1. $\mathcal{L} \{1\} = \frac{1}{s}$
2. $\mathcal{L} \{t\} = \frac{1}{s^{2}}$
3. $\mathcal{L} \{t^{n}\} = \frac{n!}{s ^{n+1}}$
4. $\mathcal{L} \{\sin(at)\} = \frac{a}{s^{2}+a^{2}}$
5. $\mathcal{L} \{\cos(at)\} = \frac{s}{s^{2}+a^{2}}$
6. $\mathcal{L} \{ e^{at} \} = \frac{1}{s-a}$
La transformada de Laplace inversa es llevar de la forma transformada a la normal.
## Transformada de la derivada
Si tenemos una función en su derivada y queremos resolver con transformada de Laplace tenemos que tener en cuenta lo siguiente:
$$
\begin{align}
\mathcal{L} \{f(t) \} = F(s)\\
\mathcal{L} \{f^{n}(t)\} =s^{n}F(s)-s ^{n-1} f(0) - s ^{n-2} f'(0) - \dots - f ^{n-1} (0)
\end{align}
$$
### Procedimiento de resolución
1. Aplicar la transformada de Laplace
2. Despejar $Y(s) = \mathcal{L} \{y(t)\}$
3. Aplicar la transformada inversa $Y(s) = \mathcal{L} \{y(t)\}$
## Teorema de traslación en el eje s
Cuando tenemos una función multiplicado por una exponencial $f(t)e^{at}$. Podemos decir lo siguiente:
$$
\mathcal{L} \{f(t)e^{at} \}=F(s)|_{s={s-a}}=F(s-a)
$$
Al resolver la transfomada de Laplace todo lo que sea $s$ se tendrá como $s-a$.
## Teorema de traslación en el eje t
La función escalón unitario es una función por partes:
$$
u(t-a)= \left\{ \begin{array}{lcc}
              0 & 0\leq t<a \\
1 & t\geq a
              \end{array}
    \right.
$$
Podemos aplicar la función unitario a funciones por partes para tenerla en solo una línea y aplicar operaciones convenientes. Por ejemplo:
$$
u(t-a)= \left\{ \begin{array}{lcc}
              0 & 0\leq t<a \\
1 & t\geq a
              \end{array}
    \right.
$$
El teorema de traslación en el eje t nos dice lo siguiente
$$
\begin{align}
\text{Si } F(s)= \mathcal{L}\{f(t) \}, a>0, \text{entonces} \\
\mathcal{L} \{f(t-a)\cdot u(t-a) \}=e^{-as}F(s) \\
\mathcal{L}^{-1} \{e^{-as}F(s) \}=f(t-a)\cdot u(t-a)
\end{align}
$$
Versión alternativa: $\mathcal{L}\{g(t)\cdot u(t-a)\}=e^{-as}\cdot \mathcal{L}\{g(t+a)\}$.
# References
- [[Semana12_Teoria_2025_1.pdf]]
- [[Semana12_Auditorio_2025_1.pdf]]
- [[Semana13_Auditorio_2025-1.pdf]]
- [[Semana13_Teoría_2025-1.pdf]]
- [[Semana14_Auditorio_2025-1.pdf]]
- [[Semana14_Teoría_2025-1.pdf]]