## Resposta Natural Criticamente Amortecida do circuito RLC

<div class="regular grid-50-50">

<div class="grid-element">

Quando consideramos a resposta criticamente amortecida de um circuito RLC, admitimos que as raízes do polinômio característico que descreve o circuito são reais e iguais. Para que este caso aconteça, o discriminante \\(\Delta\\) da equação característica deve ser igual a zero.

Até o momento, admitimos como solução para uma EDO de segunda ordem a existência de uma função \\(v(t)\\) do tipo \\(A e^{st}\\) que pode ser escrita por uma superposição de outras duas funções do tipo \\(A_{1} e^{s_{1}t}\\) e \\(A_{2} t e^{s_{2}t}\\) quando \\(s_{1} \neq s_{2}\\):

\\[
    v(t) = A_{1} e^{s_{1}t} + A_{2} e^{s_{2}t} \tag{4}
\\]

Entretanto, quando \\(s_{1} = s_{2}\\), conseguimos encontrar um sistema linear possível e determinado que encontre os valores das constantes \\(A_{1}\\) e \\(A_{2}\\)?

</div>
<div class="grid-element">

Se \\(s_{1} = s_{2}\\), então, podemos considerar \\(s_{1} = s_{2} = s\\). Substituindo \\(s_{1}\\) e \\(s_{2}\\) por \\(s\\) na equação (4), temos:

\\[
    v(t) = (A_{1} + A_{2}) e^{st} \\\\
    v^{'}(t) = s (A_{1} + A_{2}) e^{st}
\\]

Para encontrar os valores das constantes \\(A_{1}\\) e \\(A_{2}\\) temos que considerar as condições iniciais \\(v(0)\\) e \\(v^{'}(0)\\). Assim, temos que \\(v(0) = A_{1} + A_{2}\\) e \\(v^{'}(0) = s (A_{1} + A_{2})\\).

Reescrevendo este sistema na forma matricial, temos:

\\[
\begin{align}
    \begin{bmatrix}
        1 & 1 \\\\
        s & s
    \end{bmatrix}
    \cdot
    \begin{bmatrix}
        A_{1} \\\\
        A_{2} 
    \end{bmatrix}
    =
    \begin{bmatrix}
        v(0) \\\\
        v^{'}(0)
    \end{bmatrix}
\end{align}
\\]

Verificamos de imediato que a matriz dos coeficientes é singular, pois \\(det(\begin{bmatrix} 1 & 1 \\\\ s & s \end{bmatrix}) = 0\\). Portanto, o sistema linear não é determinado. Destarte, precisamos de outra função candidata \\(v(t)\\) para encontrar um SL possível e determinado que permita encontrar os valores das constantes \\(A_{1}\\) e \\(A_{2}\\).

</div>

</div>
