---
tags:
  - Math/EDO
date / time: 2025-05-30T14:22:00
Status: false
---
> [!abstract] Abstract
> Contents

---
# Conocimiento previos
En un circuito se cumple, que la caída de voltaje en estos elementos es:
- Resistencia $R$. Su voltaje es $V=RI$
- Capacitancia $C$: Su voltaje es $V=\frac{Q}{C}$
- Inductancia $L$: Su voltaje es $V=L \frac{di}{dt}$
La corriente es la derivada de la carga $I = \frac{dQ}{dt}$. Se cumplen las leyes de Kirchoff:
1. Suma de corrientes que entran es igual a la suma de corrientes que salen en un nodo.
2. La suma de caídas de voltaje en un lazo cerrado es cero.
# Circuito LC
Para un circuito LC (sin fuerza externa), la ecuación diferencial es la siguiente:
$$
\begin{align}
L\frac{di}{dt}+\frac{Q}{C}=0 \\ \\
L \frac{d^{2}q}{dt^{2}}+\frac{Q}{C} = 0
\end{align}
$$
La velocidad a la que fluye y regresa la corriente desde el condensador a la bobina se produce con una frecuencia propia $f$, denominada frecuencia de resonancia:
$$
f=\frac{\omega_{0}}{2\pi}=\frac{1}{2\pi \sqrt{ LC }}
$$
# Circuito RLC
Si el circuito no tiene una fuente entonces el $V(t)$ será 0.
$$
L \frac{d^{2}Q}{dt^{2}}+R \frac{dQ}{dt} + \frac{1}{C}Q = V(t)
$$
Si la discriminante es ($\Delta=R^{2}-\frac{4L}{C}$) se va a decir que el circuito es:
- Sobreamortiguado si $\Delta>0.$
- Críticamente amortiguado si $\Delta=0$.
- Subamortiguado si $\Delta<0$.
# References
- [[Semana10_Teoría_25_1.pdf]]
- [[Semana11_Teoria_25-1.pdf]]
- [[2024-2_Q5_1.01modB.pdf]]
- [[2024-2_Q5_1.01modA.pdf]]
- [[2024-1_Compilación QUIZ 5.pdf]]
- [[S4 - Independencia lineal y ecuaciones lineales de órden superior#Circuitos|Circuitos RC]]