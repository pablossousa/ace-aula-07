## Resposta Natural Subamortecida do circuito RLC paralelo

<div class="grid-50-50 small">

<div class="grid-element">

<!-- _class: transparent -->
![grid-img](./img/circuito-rlc-paralelo-natural.png)

Quando consideramos a resposta subamortecida de um circuito RLC, admitimos que as raízes do polinômio característico que descreve o circuito são complexas e conjugadas. Para que este caso aconteça, o discriminante da equação característica deve ser menor que zero — **ou seja, \\( \alpha^{2} - \omega_{0}^{2} < 0 \rightarrow \alpha^{2} < \omega_{0}^{2} \\)** — o que implica a existência de uma raiz quadrada de um número negativo, onde esse número pode ser escrito da forma:

Consideremos \\(s_{1}, s_{2} = -\alpha \pm \sqrt{\alpha^{2} - \omega_{0}^{2}} = -\alpha \pm j\omega_{d}\\).

É possível reescrever \\(s_{1}\\) (e \\(s_{2}\\)), por conveniência da expressão, como:

\\[
\begin{align}
    s_{1} &= -\alpha + j \omega_{d} \\\\
    s_{2} &= -\alpha - j \omega_{d}
\end{align}
\\]

</div>

<div class="grid-element">

Onde \\(\omega_{d}\\) é a frequência angular amortecida do circuito definida como:

<div class="normal" style="border: 2px solid #7851A9; padding: 5px; margin: 5px 0px;">

\\[
    \omega_{d} = \sqrt{{\omega_{0}}^{2} - \alpha^{2}}
\\]

</div>

Considerando que nossas raízes \\(s_{1}\\) e \\(s_{2}\\) são complexas e conjugadas, podemos escrever a resposta natural subamortecida do circuito RLC paralelo pela forma padrao da resposta natural como:

\\[
    v(t) = A_{1} e^{(-\alpha + j \omega_{d})t} + A_{2} e^{(-\alpha - j \omega_{d})t}
\\]

Aplicanco manipulações algébricas necessárias podemos escrever a resposta subamortecida como uma soma de senos e cossenos que oculta o termo \\(j\\) (complexo) da resposta final.

<div style="border: 2px solid #7851A9; padding: 5px; margin: 5px 0px; text-align: center;">

\\[
\begin{align}
    v(t) &= B_{1} e^{-\alpha t} \cdot \cos(\omega_{d} t) + B_{2} e^{-\alpha t} \cdot \sin(\omega_{d} t)
\end{align}
\\]

**A forma padrão da resposta natural subamortecida.**

</div>

</div>

</div>

</div>
