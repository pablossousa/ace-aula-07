## Resposta Natural do Circuito RLC Paralelo

<div class="grid-66-33 regular">

<div class="grid-element">

- Na resposta natural, estamos interessados na tensão \\(v(t)\\) do circuito. Como todos os elementos estão em paralelo \\(C, L \text{ e } R\\) sabemos que eles possuem a mesma tensão, portanto, \\(v(t)\\) nossa grandeza de interesse é partilhada por eles.

<div class="grid-50-50">

<div class="grid-element footnotesize">

- Entretanto, \\(v(t)\\) ainda é desconhecida e por sabermos que o circuito \\(RLC\\) é um circuito de segunda ordem, devemos de alguma forma encontrar expressões que possuam derivadas de \\(v(t)\\) até a segunda ordem.

</div>

<div class="grid-element footnotesize">

- Pela lei de Ohm, bem como, pelas equações de capacitância e indutância (vistas na [aula cinco](https://diegoascanio.github.io/ace-aula-05)), podemos escrever as correntes de cada um destes elementos em função de \\(v(t)\\), nossa grandeza de interesse e até então, desconhecida.

</div>

</div>

</div>

<div class="grid-element">

<!-- _class: transparent -->
![grid-img](./img/circuito-rlc-paralelo-natural.png)

</div>

</div>

<div class="grid-25-25-25-25 small">

<div class="grid-element">

Em função de \\(v(t)\\):

\\[
\begin{align}
    I_{C}(t) &= C \frac{dv(t)}{dt} \\\\
    I_{R}(t) &= \frac{v(t)}{R} \\\\
    I_{L}(t) &= \frac{1}{L} \int v(t) dt + I_{L}(0)
\end{align}
\\]

</div>

<div class="grid-element scriptsize">

Pela Lei de Kirchoff das correntes nos nós:

\\[
\begin{align}
    &I_{C}(t) + I_{R}(t) + I_{L}(t) = 0 \therefore \\\\
    &C \frac{dv(t)}{dt} + \frac{v(t)}{R} + \frac{1}{L} \int v(t) dt + I_{L}(0) = 0
\end{align}
\\]


</div>

<div class="grid-element tiny">

Podemos derivar os dois lados da equação à esquerda em relação ao tempo \\(t\\):

\\[
\begin{align}
    \frac{d}{dt} &\left( C \frac{dv(t)}{dt} + \frac{v(t)}{R} \right. \\\\ 
    &\left. + \frac{1}{L} \int v(t) dt + I_{L}(0) \right) = 0 \therefore \\\\
    &C \frac{d^{2}v(t)}{dt^{2}} + \frac{1}{R} \frac{dv(t)}{dt} + \frac{1}{L} v(t) = 0
\end{align}
\\]

\\(I_{L}(0)\\) é constante, portanto, \\(\frac{d}{dt} I_{L}(0) = 0\\).

</div>

<div class="grid-element footnotesize">

Já encontramos a derivada de segunda ordem de \\(v(t)\\), como esperávamos, agora, multiplicamos a equação por \\(1 \over C\\) e obtemos:

\\[
\begin{align}
    &\frac{d^{2}v(t)}{dt^{2}} + \frac{1}{RC} \frac{dv(t)}{dt} + \frac{1}{LC} v(t) = 0
\end{align}
\\]

</div>

</div>
