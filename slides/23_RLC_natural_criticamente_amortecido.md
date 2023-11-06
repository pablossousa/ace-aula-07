## Resposta Natural Criticamente Amortecida do circuito RLC

<div class="regular">

Considerando que \\(s_{1} = s_{2} = s = - \alpha = -\frac{1}{2RC} \\) precisamos encontrar função (funções) candidata(s) para \\(v(t)\\) que forme(m) um conjunto fundamental de soluções para a equação diferencial homogênea que sejam linearmente independentes, para que \\(D_{1} (A_{1}) \neq -D_{2} (A_{2})\\) e portanto, outra solução além da trivial — \\(v(t) = 0\\) \\(\forall t \geq 0 \\), físicamente inviável  — seja possível.

Considerar \\(v(t) = (D_{1}t + D_{2})e^{st}\\) forma este conjunto de soluções fundamentais? Vamos verificar.

</div>

<div class="small grid-50-50" style="border-style: solid; border-width: 2px; border-color: #6b3fa0;">

<div class="grid-element">

\\[
\begin{align}
    v(t) &= (D_{1}t + D_{2})e^{st} \\\\
    \frac{d v(t)}{dt} &= (st + 1) \cdot D_{1}e^{st} + s \cdot D_{2}e^{st} 
\end{align}
\\]

Para encontrarmos \\(D_{1}\\) e \\(D_{2}\\) temos de considerar \\(v(0)\\) e \\(\frac{dv(0)}{dt}\\). Assim:

\\[
\begin{align}
    v(0) &= (D_{1} \cdot 0 + D_{2})e^{s \cdot 0} = D_{2} \\\\
    \frac{dv(0)}{dt} &= (s \cdot 0 + 1) \cdot D_{1}e^{s \cdot 0} + s \cdot D_{2}e^{s \cdot 0} = D_{1} + s \cdot D_{2}
\end{align}
\\]

Reescrevendo este sistema em sua representação matricial, temos:

\\[
\begin{align}
\begin{bmatrix}
0 & 1 \\\\
1 & s
\end{bmatrix}
\cdot
\begin{bmatrix}
D_{1} \\\\
D_{2}
\end{bmatrix}
&=
\begin{bmatrix}
v(0) \\\\
\frac{dv(0)}{dt}
\end{bmatrix}
\end{align}
\\]

</div>

<div class="grid-element">

Agora, verificamos que \\(det(
\begin{bmatrix}
0 & 1 \\\\
1 & s
\end{bmatrix}) \neq 0
\\) em qualquer situação, o que portanto, garante um sistema linear possível e determinado para encontrar os valores de \\(D_{1}\\) e \\(D_{2}\\) que serão, respectivamente:

\\[
\begin{align}
D_{1} &= \frac{dv(0)}{dt} - s \cdot v(0) \\\\
D_{2} &= v(0)
\end{align}
\\].

Resta verificar agora se \\(\frac{d^{2}v(t)}{dt^{2}} + \frac{1}{RC} \frac{dv(t)}{dt} + \frac{1}{LC}v(t) = 0\\) quando \\(v(t) = (D_{1}t + D_{2})e^{st}\\).

Utilizaremos o exemplo 8.5 do livro de NILSSON, RIEDEL 10ªed. implementado em um jupyter notebook no próximo slide para fazer esta verificação.

</div>

</div>
