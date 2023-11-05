## Formas de resposta natural de um circuito \\(RLC\\) paralelo — Resposta Superamortecida

<div class="grid-50-50 regular">

<div class="grid-element">

- Recapitulando: ocorre quando as raízes da equação característica são reais e distintas.

- A solução para \\(v(t)\\) tem a forma

\\[
    v(t) = A_{1} e^{s_{1} t} + A_{2} e^{s_{2} t}
\\]

- Para determinar as constantes \\(A_{1}\\) e \\(A_{2}\\), precisamos das condições iniciais do circuito, dadas pelos valores de \\(v(0^{+})\\) e \\(\frac{dv(0^{+})}{dt}\\) que por sua vez, são determinados pela tensão inicial no capacitor, \\(V_{0}\\), e pela corrente inicial no indutor, \\(I_{0}\\).

</div>

<div class="grid-element">

Considerando \\(v(0^{+})\\), temos:

\\[
    v(0^{+}) = A_{1} e^{s_{1} \times 0} + A_{2} e^{s_{2} \times 0} = A_{1} + A_{2}
\\]

Ao fazermos a primeira derivada, temos:

\\[
    \frac{dv(t)}{dt} = A_{1} s_{1} e^{s_{1} t} + A_{2} s_{2} e^{s_{2} t}
\\]

Substituindo \\(t = 0^{+}\\), temos:

\\[
\begin{align}
    \frac{dv(0^{+})}{dt} &= A_{1} s_{1} e^{s_{1} \times 0} + A_{2} s_{2} e^{s_{2} \times 0} \therefore \\\\
    \frac{dv(0^{+})}{dt} &= s_{1} A_{1} + s_{2} A_{2}
\end{align}
\\]

Se conhecermos \\(s_{1}\\) e \\(s_{2}\\), encontrar \\(A_{1}\\) e \\(A_{2}\\) limita-se a:
1. Determinar \\(v(0^{+})\\) e \\(\frac{dv(0^{+})}{dt}\\);
2. Resolver o sistema linear resultante.

</div>

</div>
