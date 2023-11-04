## Resposta Natural do Circuito RLC Paralelo - Solução Geral da Equação Diferencial de Segunda Ordem

<div class="grid-50-50 regular">

<div class="grid-element">

É conveniente escrever \\(s_{1} e s_{2}\\) em função dos parâmetros \\(\alpha \text{ e } \omega_{0}\\) para interpretar o comportamento do circuito em relação a seus parâmetros \\(RLC\\) e de suas características — superamortecimento, subamortecimento e amortecimento crítico — que serão estudadas adiante. 

Considerando \\(\alpha = \frac{1}{2RC}\\) e \\(\omega_{0} = \frac{1}{\sqrt{LC}}\\), temos:

\\[
\begin{align}
    s_{1} &= -\alpha + \sqrt{\alpha^{2} - \omega_{0}^{2}} \\\\
    s_{2} &= -\alpha - \sqrt{\alpha^{2} - \omega_{0}^{2}} 
\end{align}
\\]

Os parâmetros \\(\alpha \text{ e } \omega_{0}\\) são conhecidos respectivamente por frequência de néper (ou fator de amortecimento) e frequência angular de ressonância (ou fator de oscilação) e eles que ditarão as características do circuito (superamortecimento, subamortecimento e amortecimento crítico).

</div>

<div class="grid-element">

A tabela abaixo apresenta um resumo destes parâmetros para facilitar o entendimento:

<div class="scriptsize" style="width: 80%; margin: auto; text-align: center;">

<!-- _class: ttable -->
|      Parâmetro     |              Terminologia             |                      Valor (na resposta natural)                    |      Unidade      |
|:------------------:|:-------------------------------------:|:-------------------------------------------------------------------:|:-----------------:|
| \\(s_{1}, s_{2}\\) |    Raízes da equação característica   | \\(s_{1}, s_{2} = -\alpha \pm \sqrt{\alpha^{2} - \omega_{0}^{2}}\\) |\\(\frac{rad}{s}\\)|
|  \\(\alpha\\)      |          Frequência de néper          |                \\( \alpha = \frac{1}{2RC} \\)                       |\\(\frac{rad}{s}\\)|
| \\(\omega_{0}\\)   |   Frequência angular de ressonância   |           \\( \omega_{0} = \frac{1}{\sqrt{LC}} \\)                  |\\(\frac{rad}{s}\\)|

</div>

Porque as unidades de todos os parâmetros estão em \\(\frac{rad}{s}\\)? Porque as raízes \\(s_{1}\\) e \\(s_{2}\\) (e por consequência, os parâmetros \\(\alpha \text{ e } \omega_{0}\\) que as determinam) são coeficientes do tempo \\(t\\) na exponencial \\(e^{st}\\). Como o expoente de \\(e\\) deve ser adimensional, logo, \\(s\\) deve ter a dimensão do recíproco (neste caso, inverso) do tempo — a frequência — para manter o expoente de \\(e^{st}\\) adimensional.

</div>

</div>
