<style>
  section {
    background: #fff url(./img/background.png) no-repeat center center;
    background-size: cover;
  }

  section.center img {
    display: block;
    margin: auto;
  }

  img[alt=small-img] {
    display: block;
    margin: auto;
    width: 30%;
  }

  .transparent {
    background-color: transparent!important;
  }

  section.transparent img {
    background-color: transparent!important;
  }

  section.ttable table {
    margin: auto;
  }

  .cabecalho {
    position: absolute;
    top: 10%;
    margin-left: 5%;
    margin-right: 10%;
    font-size: 48px;
    font-weight: bold;
  }

  .conteudo {
    top: 30%;
    margin-left: 5%;
    margin-right: 10%;
    font-size: 28px;
    text-align: justify;
  }

  .conteudo-absoluto {
    position: absolute;
    top: 30%;
    margin-left: 5%;
    margin-right: 10%;
    font-size: 28px;
    text-align: justify;
  }
  
  .large {
    font-size: 36px;
  }

  .normal {
    font-size: 22px;
  }
  .regular {
    font-size: 18px;
  }
  .small {
    font-size: 16px;
  }
  .footnotesize {
    font-size: 14px;
  }
  .scriptsize {
    font-size: 12px;
  }
  .tiny {
    font-size: 10px;
  }
  .bold {
    font-weight: bold;
  }
  .center {
    text-align: center;
  }
  section.lead p {
    text-align: justify;
  }
  section.lead h1 {
    text-align: center;
  }
  section.lead h2 {
    text-align: center;
  }
  section.lead h3 {
    text-align: center;
  }
  
  .grid-50-50 {
    display: grid;
    grid-template-columns: 1fr 1fr;
    text-align: justify;
  }

  .grid-25-25-25-25 {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    text-align: justify;
  }

  .grid-33-33-33 {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    text-align: justify;
  }


  .grid-66-33 {
    display: grid;
    grid-template-columns: 2fr 1fr;
    text-align: justify;
  }

  .grid-33-66 {
    display: grid;
    grid-template-columns: 1fr 2fr;
    text-align: justify;
  }

  .grid-element {
    margin-left: 5%;
    margin-right: 5%;
  }
  img[alt=grid-img] {
    width: 100%;
  }

</style>

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>


# Seminário - Análise de Circuitos Elétricos
# Grupo 1  - As características da resposta subamortecida natural
 
Gabriel Teixeira Júlio (gabriel.julio@aluno.cefetmg.br), Marcus Vinicius Nogueira Santos (marcuscefet@gmail.com), Mateus Henrique Pereira (mateus@aluno.cefetmg.br) e Pablo Sousa da Silva (pablossilva.005@gmail.com)

Aula baseada sobre o material do professor Dr. Emerson Gonçalves de Melo (emerdemelo@usp.br - DEMAR EEL USP), da professora Drª. Thabatta Moreira Alves de Araújo (thabatta@cefetmg.br - DIGDDV), do professor M.Sc. Diego Ascânio Santos (ascanio@cefetmg.br) e da Khan Academy.

CEFET-MG DIGDDV - Divinópolis, 2023.


---

## Roteiro

1. Respota natural de um circuito RLC em paralelo subamortecido.
2. Características da resposta subamortecida natural.


---

## Objetivos

1. Saber a resposta natural de circuitos RLC em paralelo subaortecido.
2. Saber as características da resposta subamortecida natural.


---

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


---

## Características da resposta subamortecida natural

<div class="grid-50-50 small">

<div class="grid-element">

A resposta subamortecida em circuitos RLC é caracterizada por oscilações que diminuem gradualmente ao longo do tempo. Ela ocorre quando a resistência no circuito é relativamente baixa, resultando em um fator de amortecimento menor que 1. Algumas características importantes da resposta subamortecida natural em circuitos RLC:

1. **Oscilações Sobrepostas:** A resposta subamortecida resulta em oscilações que sobrepujam a resposta transitória e persistem por algum tempo antes de eventualmente atenuarem. Essas oscilações são caracterizadas por picos e vales.

2. **Frequência Natural (\\(\omega_{0}\\)):** A frequência natural do sistema é a frequência das oscilações não amortecidas. É determinada pelos valores dos componentes no circuito (resistor, indutor e capacitor) e é dada por \\(\omega_{0} = \frac{1}{\sqrt{LC}}\\) , onde L é a indutância e C é a capacitância.

</div>

<div class="grid-element">

<!-- _class: transparent -->
![grid-img](./img/grafico-subamortecida.png)

</div>


</div>

---

## Características da resposta subamortecida natural

<div class="grid-50-50 small">

<div class="grid-element">

3. **Fator de Amortecimento (\\(\zeta\\)):** O fator de amortecimento é uma medida da quantidade de amortecimento presente no sistema. Para a resposta subamortecida, o fator de amortecimento é  \\(0 < \zeta < 1\\). É determinada pelos valores dos componentes no circuito (resistor, indutor e capacitor) e é dado por \\(\zeta = \frac{R}{2L\omega_{0}}\\), onde R é a resistência e L é a indutância.

4. **Tempo de Subida (\\(T_{r}\\)):** O tempo de subida é o tempo necessário para a resposta atingir aproximadamente 63,2% do valor final após uma mudança no sinal de entrada. Para sistemas subamortecidos, o tempo de subida é menor em comparação com sistemas superamortecidos. É determinado por \\(T_{r} = \frac{1}{\zeta\omega_{0}}\\), onde \\(\zeta\\) é o fator de amortecimento e \\(\omega_{0}\\) é a frequência natural.  

</div>

<div class="grid-element">

<!-- _class: transparent -->
![grid-img](./img/grafico-subamortecida.png)

</div>


</div>

---

## Características da resposta subamortecida natural

<div class="grid-50-50 small">

<div class="grid-element">

5. **Ressonância:** Pode ocorrer ressonância se a frequência da fonte de entrada coincidir com a frequência natural do sistema. Isso pode resultar em picos mais pronunciados na resposta do sistema.

6. **Amplitude Máxima (Overshoot)\\((\\%OS)\\):**  resposta subamortecida geralmente exibe um overshoot, que é a porcentagem pela qual a resposta ultrapassa o valor final antes de se estabilizar. O overshoot é maior em sistemas subamortecidos em comparação com sistemas criticamente amortecidos. É determinado por \\(\\%OS = 100 . e^{-\frac{\zeta\pi}{\sqrt{1-\zeta^2}}}\\), onde \\(\zeta\\) é o fator de amortecimento.

</div>

<div class="grid-element">

<!-- _class: transparent -->
![grid-img](./img/grafico-subamortecida.png)

</div>


</div>

---

## Características da resposta subamortecida natural

<div class="grid-50-50 small">

<div class="grid-element">

7. **Tempo de Estabilização \\((T_{s})\\):** O tempo de estabilização é o tempo necessário para que a resposta atinja e permaneça dentro de uma faixa aceitável ao redor do valor final. Para sistemas subamortecidos, o tempo de estabilização pode ser maior em comparação com sistemas criticamente amortecidos. Ele pode ser dividido em 3 tipos:

- 4% - Maior oscilação no valor final:

\\[
\begin{align}
T_{s} = \frac{3,2}{\zeta\omega_{0}}
\end{align}
\\]

- 3% - Média oscilação no valor final:

\\[
\begin{align}
T_{s} = \frac{3,5}{\zeta\omega_{0}}
\end{align}
\\]

- 2% - Menor oscilação no valor final:

\\[
\begin{align}
T_{s} = \frac{4}{\zeta\omega_{0}}
\end{align}
\\]

</div>

<div class="grid-element">

<!-- _class: transparent -->
![grid-img](./img/grafico-subamortecida.png)

</div>


</div>

---

<div class="cabecalho large">
Referências Bibliográficas
</div>
<div class="conteudo normal">

- RIEDEL, SUSAN A.; NILSSON, James W. — Circuitos Elétricos 8ª ed. 2009.
- RIEDEL, SUSAN A.; NILSSON, James W. — Circuitos Elétricos 10ª ed. 2015.
- DE MELO, E. G. — Curso: LOM3202 - Circuitos Elétricos (2020). Accessed August 6, 2023. https://edisciplinas.usp.br/course/view.php?id=82680.
- DE ARAÚJO, THABATTA M. A. - SLIDES E NOTAS DE AULAS - Disponível junto à profª Thabatta.

</div>
