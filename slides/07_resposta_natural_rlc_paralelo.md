## Resposta Natural do Circuito RLC Paralelo - Solução Geral da Equação Diferencial de Segunda Ordem

<div class="grid-50-50 regular">

<div class="grid-element">

Recapitulando nossa EDO de ordem 2, temos:

\\[
\begin{align}
    &\frac{d^{2}v(t)}{dt^{2}} + \frac{1}{RC} \frac{dv(t)}{dt} + \frac{1}{LC} v(t) = 0 \tag{1} \label{eq:edo_{2}}\\
\end{align}
\\]

Pela nossa EDO ser de segunda ordem, não podemos solucioná-la pelo método da separação de variáveis para EDOs homogêneas de ordem 1. Mas, sabemos que toda EDO tem por solução uma função exponencial em função de \\(t\\). Consideremos \\(v(t)\\) como

\\[
    v(t) = A e^{st}
\\]

É \\(A e^{st}\\) uma função candidata para solucionar nossa EDO representada pela equação 1? Para descobrirmos, vamos substituir \\(v(t)\\) na equação 1 por \\(A e^{st}\\):


</div>

<div class="grid-element footnotesize">

<!-- _class: center -->
### Substituindo \\(v(t)\\) por \\(A e^{st}\\) na equação 1

\\[
\begin{align}
    &\frac{d^{2}(A e^{st})}{dt^{2}} + \frac{1}{RC} \frac{d(A e^{st})}{dt} + \frac{1}{LC} (A e^{st}) = 0 \therefore \\\\
    &A s^{2} e^{st} + \frac{1}{RC} A s e^{st} + \frac{1}{LC} A e^{st} = 0 \therefore \\\\
    &A e^{st} \left( s^{2} + \frac{s}{RC} + \frac{1}{LC} \right) = 0 \tag{2} \label{edo:caract} \\
\end{align}
\\]

Estudando a equação 2, 

\\[A e^{st} \left( s^{2} + \frac{s}{RC} + \frac{1}{LC} \right) = 0 \leftrightarrow A = 0 \text{ ou } {s^2 + \frac{s}{RC} + \frac{1}{LC} = 0} \\]

Pois, \\(e^{st} \neq 0 \text{ } \forall t\\). Se \\(A\\) for nulo, isso implica que \\(v(t) = 0 \text{ } \forall t\\) o que é fisicamente impossível na ocasião em que exista energia armazenada nos elementos do circuito em seu estado inicial, implicando assim que \\(A\\) seja não nulo para generalizar! Logo, \\(A e^{st}\\) é solução candidata para a solução da EDO de ordem 2 quando \\(s^2 + \frac{s}{RC} + \frac{1}{LC} = 0\\). 

O termo \\(s^2 + \frac{s}{RC} + \frac{1}{LC}\\) é chamado de **equação característica** da EDO de ordem 2 e suas raízes \\(s_{1}\\) e \\(s_{2}\\), chamadas de **raízes características** da EDO de ordem 2, fazem com que seja possível encontrar soluções da forma \\(v(t) = A e^{s_{1}t}\\) e \\(v(t) = B e^{s_{2}t}\\) para a EDO de ordem 2.

</div>

</div>
