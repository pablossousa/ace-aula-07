## Formas de resposta natural de um circuito \\(RLC\\) paralelo — Resposta Superamortecida

<div class="regular">

O processo para determinação da resposta superamortecida \\(v(t)\\) pode ser resumido da seguinte forma — ipsis líteris ao contido em NILSSON, RIEDEL 10ª Edição p. 298:

1. Determine as raízes da equação característica \\(s_{1}\\) e \\(s_{2}\\), usando os valores de \\(R, L \text{ e } C\\);
2. Determine \\(v(0^{+})\\) e \\(\frac{dv(0^{+})}{dt}\\) usando análise de circuitos;
3. Determine os valores de \\(A_{1}\\) e \\(A_{2}\\) usando as equações simultaneamente:
\\[
\begin{align}
v(0^{+}) &= A_{1} + A_{2} \\\\
\frac{dv(0^{+})}{dt} &= \frac{i_{C}(0^{+})}{C} = s_{1}A_{1} + s_{2}A_{2}
\end{align}
\\]
4. Substitua os valores de \\(s_{1}, s_{2}, A_{1} \text{ e } A_{2}\\) na equação da resposta natural \\(v(t) = A_{1}e^{s_{1}t} + A_{2}e^{s_{2}t}\\) para determinar \\(v(t), t \geq 0\\).

Resolveremos dois exemplos (8.2, 8.3) presentes no livro de NILSSON, RIEDEL 10ª Edição p. 298-300 para ilustrar o processo de determinação da resposta superamortecida.

</div>
