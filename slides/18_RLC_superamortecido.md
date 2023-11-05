## Formas de resposta natural de um circuito \\(RLC\\) paralelo — Resposta Superamortecida

<div class="grid-50-50 regular">

<div class="grid-element">

Se conhecermos \\(s_{1}\\) e \\(s_{2}\\), encontrar \\(A_{1}\\) e \\(A_{2}\\) limita-se a:
1. Determinar \\(v(0^{+})\\) e \\(\frac{dv(0^{+})}{dt}\\);
2. Resolver o sistema linear resultante.

</div>

<div class="grid-element">

<!-- _class: transparent center -->
![](./img/circuito-rlc-paralelo-natural.png)

</div>

</div>

<div class="grid-33-33-33 footnotesize">

<div class="grid-element">

- O valor \\(v_{0^{+}}\\) é a tensão \\(V_{0}\\) no capacitor no instante \\(t=0^{+}\\);
- Pelas equações da capacitância:

\\[
\begin{align}
    i_{C}(0^{+}) &= C \frac{dv_{0^{+}}}{dt} \therefore \\\\
    \frac{dv_{0^{+}}}{dt} &= \frac{i_{C}(0^{+})}{C} \tag{3}
\end{align}
\\]

</div>

<div class="grid-element">

- Assim, temos que determinar qual a corrente \\(i_{C}(0^{+})\\) que circula no capacitor no instante \\(t=0^{+}\\);
- Pela Lei de Kirchoff das Correntes nos nós, temos que \\(0 = i_{C} + i_{L} + i_{R} \\);
- Pela Lei de Ohm, temos que \\(i_{R} = \frac{V_{0}}{R}\\);
- A corrente presente no indutor no instante de tempo \\(t=0^{+}\\) é \\(I_{0}\\);

</div>

<div class="grid-element">

- Reorganizando a equação obtida pela LKC nos nós obtém-se: \\(i_{C} = -i_{R} - i_{L}\\);
- Substituindo-se \\(I_{R}\\) por \\(\frac{V_{0}}{R}\\) e \\(I_{L}\\) por \\(I_{0}\\), temos que \\(i_{C} = -\frac{V_{0}}{R} - I_{0}\\);
- Assim, podemos determinar o valor numérico de \\(i_{C}(0^{+})\\) e substituir na equação (3) para determinar \\(\frac{dv_{0^{+}}}{dt}\\).
- Depois, substituimos \\(v_{0^{+}}\\) e \\(\frac{dv_{0^{+}}}{dt}\\) no sistema linear e o resolvemos, obtendo \\(A_{1}\\) e \\(A_{2}\\).

</div>

</div>
