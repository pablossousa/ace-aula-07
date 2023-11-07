## Resposta Natural Subamortecida do circuito RLC paralelo

<div class="grid-50-50 small">

<div class="grid-element">

A partir de

\\[
\begin{align}
    v(t) &= A_{1} e^{(-\alpha + j \omega_{d})t} + A_{2} e^{(-\alpha - j \omega_{d})t} \\\\
    &\text{Temos: } \\\\
    &= A_{1} e^{-\alpha t} e^{j \omega_{d} t} + A_{2} e^{-\alpha t} e^{-j \omega_{d} t} \therefore \\\\
    &= e^{-\alpha t} \left( A_{1} e^{j \omega_{d} t} + A_{2} e^{-j \omega_{d} t} \right) \\\\
    &\text{Aplicando a identidade de Euler: } \\\\
    &= e^{-\alpha t} \left( A_{1} \cos(\omega_{d} t) + j A_{1} \sin(\omega_{d} t) + \right. \\\\ 
    &\left. A_{2} \cos(\omega_{d} t) - j A_{2} \sin(\omega_{d} t) \right) \\\\
    &= e^{-\alpha t} \left[ (A_{1} + A_{2}) \cdot \cos(\omega_{d} t) + \right. \\\\
    &\left. j (A_{1} - A_{2}) \cdot \sin(\omega_{d} t) \right] 
\end{align}
\\]

</div>

<div class="grid-element">

Agora, substitua as constantes arbitrárias \\( A_{1} + A_{2} \\) e \\( j (A_{1} - A_{2}) \\) por novas constantes reais arbitrárias denotadas \\( B_{1} \\) e \\( B_{2} \\), respectivamente, para obter:

\\[
\begin{align}
    v(t) &=  e^{-\alpha t} \left[ B_{1} \cdot \cos(\omega_{d} t) + B_{2} \cdot \sin(\omega_{d} t) \right] \therefore \\\\
\end{align}
\\]

<div style="border: 2px solid #7851A9; padding: 5px; margin: 5px 0px; text-align: center;">

\\[
\begin{align}
    v(t) &= B_{1} e^{-\alpha t} \cdot \cos(\omega_{d} t) + B_{2} e^{-\alpha t} \cdot \sin(\omega_{d} t)
\end{align}
\\]

**A forma padrão da resposta natural subamortecida.**

</div>

Observações:
- Não se deixe enganar pelo fato de que \\(B_{2} = j(A_{1} - A_{2})\\). Neste caso, \\(A_{1}\\) e \\(A_{2}\\) são conjugados complexos, de modo que \\(B_{1}, B_{2}\\) são reais, de acordo com Nilsson Riedel 10ª edição.
    - Quem provar matematicamente que \\(B_{1}, B_{2}\\) são reais ganha 3 pontos extras, quero a prova formatada em LaTeX.

</div>

</div>
