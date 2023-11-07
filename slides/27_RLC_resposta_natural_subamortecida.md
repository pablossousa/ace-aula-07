## Resposta Natural Subamortecida do circuito RLC paralelo

<div class="grid-50-50 small">


<div class="grid-element">

Conhecendo a forma geral da resposta Subamortecida de um circuito \\(RLC\\) paralelo dada por:

\\[
    v(t) =  e^{-\alpha t} \left[ B_{1} \cdot \cos(\omega_{d} t) + B_{2} \cdot \sin(\omega_{d} t) \right]
\\]

Devemos agora determinar \\(B_{1}\\) e \\(B_{2}\\). Para a resposta subamortecida, as duas equações simultâneas que determinam \\(B_{1}\\) e \\(B_{2}\\) dependem das condições iniciais \\(v(0^{+})\\) e \\(\frac{dv(0^{+})}{dt}\\) do circuito, sendo:

\\[
\begin{align}
v(0^{+}) &= V_{0} = B_{1} \\\\
\frac{dv(0^{+})}{dt} = \frac{i_{C}(0^{+})}{C} = - \alpha B_{1} + \omega_{d} B_{2}
\end{align}
\\]


</div>

<div class="grid-element">

Verificaremos no exemplo 8.4 — NILSSON, RIEDEL 10ª Ed. — que a resposta subamortecida de um circuito é caracterizada por oscilações indicadas por funções trigonométricas, com a tensão alternando entre valores positivos e negativos. A frequência dessas oscilações é determinada por \\(\omega_{d}\\), enquanto a taxa de diminuição da amplitude é regida pelo fator de amortecimento \\(\alpha\\). A frequência \\(\omega_{d}\\) é conhecida como a frequência angular amortecida, que é menor do que a frequência natural \\(\omega_{0}\\) em presença de um elemento dissipativo \\(R\\) no circuito. Quando \\(\alpha \neq 0\\), a frequência de oscilação é considerada amortecida.

</div>

</div>
