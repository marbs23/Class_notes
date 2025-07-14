---
tags:
  - Math/EDO
date / time: 2025-05-26T07:01:00
Status: false
---
> [!abstract] Abstract
> Contents

---
# Conceptos clave:
- 2da ley de Newton $F = ma$: La fuerza neta (suma de todas las fuerzas) del sistema es proporcional a la masa del objeto por su aceleración.
- Sistema en reposo: Si un sistema está en reposo las fuerzas que apuntan hacia la derecha son iguales a las fuerzas que apuntan a la izquierda. Así mimso, las fuerzas que apuntan hacia arriba son iguales a las fuerzas que apuntan hacia abajo.
- Ley de Hooke $F=kx$: La fuerza restauradora de un resorte es proporcional a cúanto se estira o comprime el resorte ($x$), dónde $k$ es la constante del resorte.
- Signos en base al movimiento: cuando una fuerza favorece el movimiento de un objeto el signo de la fuerza es positivo y cuando va en dirección opuesta es negativo.
# Sistema Masa Resorte
## Sistema Masa Resorte sin Amortiguamiento
En un sistema masa resorte analizamos la dinámica de un objeto de masa $m$ sujetado por un resorte con constante $k$.
Un objetido suspendido en reposo verticalmente y sujeto por un resorte se puede decir $mg = ks$. Dónde $s$ es la distancia del resorte desde el resorte sin ser deformado hasta el momento en que el objeto está en reposo.
Al analizar la dinámica bajo la segunda ley de Newton se tiene lo siguiente:
$$
\begin{align}
m\ddot{x} &= -k(s+x)+mg \\
m\ddot{x} &= -ks-kx+mg \\
m\ddot{x} &= -kx \\
m\ddot{x} +kx&= 0 \\
\ddot{x} +w^{2}x&= 0
\end{align}
$$
- $x$ será la distancia del objeto desde el momento de reposo hasta un tiempo $t$.
- Tener en cuenta que la fuerza restauradora del resorte es negativa porque se opone a la dirección del movimiento del objeto.
- $w^{2}=\frac{k}{m}$
## Sistema Masa Resorte con Amortiguamiento
En un sistema masa resorte aparte de existir un objeto sujeto a un resorte existe una fuerza que reduce poco a poco el movimiento del sistema. Se considera que las fuerzas de amortiguamiento al sistema son proporcionales a la velocidad instantánea del objeto $\gamma \dot{x}$, dónde $\gamma$ es la constante de amortiguamiento.
Analizando la dinámica del sistema:
$$
\begin{align}
m \ddot{x} &= mg - k(s+x) -\gamma \dot{x} \\
m \ddot{x} &= -kx -\gamma \dot{x} \\
0 &= m \ddot{x} +kx +\gamma \dot{x}
\end{align}
$$
# Modelos con múltiples resortes y masas
## Una masa y dos resortes
En un sistema con una masa y 2 resortes se debe analizar 3 momentos del sistema:
1. Cuando las longitudes de los resortes no son modificadas
2. Cuando el sistema está en resposo
3. Cuando el sistema está en movimiento
Si el sistema es amortiguado tenemos que recordar que el amortiguamiento va en contra del movimiento del objeto y es proporcional a la velocidad con la que se mueve el objeto $(-cx')$.
$$
\begin{align}
m\ddot{x}+(K_{1}+K_{2})x=& 0 \\
m\ddot{x}+ c\dot{x}+ (K_{1}+K_{2})x=& 0
\end{align}
$$
## Dos masas y tres resortes
En un sistema con dos masas y 3 resortes las posiciones son medidas respecto a la posición de equilibrio y se analizan 2 momentos:
1. Cuando el sistema está en reposo
2. Cuando el sistema está en movimiento
Los diagramas de cuerpo libre en movimiento son analizados por separado siendo el movimiento de la masa de la izquierda $x$ y el movimiento de la masa de la derecha $y$. Al moverse a la derecha, el resorte 1 es estirado $x$, el resorte 2 es estirado $y-x$ y el resorte 3 es comprimido $y$. **Así mismo, tener cuidado con las constantes de los resortes porque pueden ser distintas**. En caso de ser iguales tenemos el siguiente sistema de ecuaciones diferenciales.
$$
\begin{align}
m \ddot{x} + 2kx - ky = 0\\
m \ddot{y} + 2ky - kx = 0
\end{align}
$$
En caso de un sistema con amortiguamiento el siguiente sistema:
$$
\begin{align}
m \ddot{x} + c \dot{x} + 2kx - ky = 0\\
m \ddot{y} + c \dot{y} + 2ky - kx = 0
\end{align}
$$

> [!tip] Consejo para sistemas masa resorte
> En los sistemas masa resorte analizar de acuerdo a los principios físicos de ley de hooke, posición de equilibrio y segunda ley de Newton. En el movimiento entre 2 resortes solo darse cuenta de cuánto se mueve el resorte de la posición de equilibrio en cada extremo de cada resorte.

# References
- [[Semana09_Teoría_25_1.pdf]]
- [[Semana10_Auditorio_25_1.pdf]]
- [[Semana11_Auditorio_25-1.pdf]]