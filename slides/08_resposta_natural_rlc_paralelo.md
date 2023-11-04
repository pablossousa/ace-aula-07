## Resposta Natural do Circuito RLC Paralelo - Solução Geral da Equação Diferencial de Segunda Ordem

<div class="grid-50-50 regular">

<div class="grid-element">

A equação \\(s^2 + \frac{s}{RC} + \frac{1}{LC} = 0\\) é chamada de **equação característica** da EDO de ordem 2 porquê suas raízes \\(s_{1}\\) e \\(s_{2}\\) determinam o caráter matemático de \\(v(t)\\).

Para encontrar suas raízes, apenas resolvemos esta equação de segundo grau pela fórmula de Bhaskara:

\\[s_{1,2} = \frac{-\frac{1}{RC} \pm \sqrt{\left(\frac{1}{RC}\right)^2 - 4\frac{1}{LC}}}{2}\\]

Aplicando as manipulações algébricas adequdas temos que:

\\[
\begin{align}
    s_{1} &= -\frac{1}{2RC} + \sqrt{\left(\frac{1}{2RC}\right)^2 - \frac{1}{LC}} \\\\
    s_{2} &= -\frac{1}{2RC} - \sqrt{\left(\frac{1}{2RC}\right)^2 - \frac{1}{LC}}
\end{align}
\\]

</div>

<div class="grid-element">

Se substituirmos \\(s\\) por \\(s_{1}\\) ou \\(s_{2}\\) na equação \\(v(t) = Ae^{st}\\), a solução satisfaz a EDO descrita pela equação [1](#7), pois, para qualquer valor de \\(A\\), \\(s^{2} + \frac{s}{RC} + \frac{1}{LC} = 0\\) quando \\(s = s_{1}\\) ou \\(s = s_{2}\\), já que \\(s_{1}, s_{2}\\) são raízes da equação característica.

Considere agora \\(v_{1}(t) = A_{1}e^{s_{1}t}\\) e \\(v_{2}(t) = A_{2}e^{s_{2}t}\\) como soluções da EDO [1](#7). A soma \\(v(t) = v_{1}(t) + v_{2}(t)\\) também é solução da EDO (demonstração presente no livro do Riedel 8ª edição).

Destarte, a solução geral da resposta natural do circuito \\(RLC\\) é dada por:

<div style="box-sizing: border-box; border: 3px dotted #7851A9;">

\\[
    V(t) = A_{1}e^{s_{1}t} + A_{2}e^{s_{2}t}
\\]

</div>



</div>

</div>
