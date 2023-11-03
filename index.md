<style>
  section {
    background: #fff url(./img/background.png) no-repeat center center;
    background-size: cover;
  }

  .transparent {
    background-color: transparent!important;
  }

  section.transparent img {
    background-color: transparent!important;
  }

  .transparent-table-tr-td-th {
    background-color: rgba(0, 0, 0, 0.0) !important;
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


# Análise de Circuitos Elétricos
## Aula 07 - Respostas natural e a um degrau em circuitos de segunda ordem (RLC)
 
Prof. M.Sc. Diego Ascânio Santos (ascanio@cefetmg.br)

Aula baseada sobre o material do professor Dr. Emerson Gonçalves de Melo (emerdemelo@usp.br - DEMAR EEL USP), da professora Drª. Thabatta Moreira Alves de Araújo (thabatta@cefetmg.br - DIGDDV) e da Khan Academy.

CEFET-MG DIGDDV - Divinópolis, 2023.


---

## Roteiro

1. Introdução à resposta natural de um circuito RLC em paralelo.
2. Formas de resposta natural de um circuito RLC em paralelo.
3. Resposta a um degrau de um circuito RLC em paralelo.
4. Respostas natural e a um degrau de um circuito RLC em série.


---

## Objetivos

1. Saber determinar a resposta natural e a resposta a um degrau de circuitos RLC em paralelo.
2. Saber determinar a resposta natural e a resposta a um degrau de circuitos RLC em série.


---

## Introdução - Circuitos de Segunda Ordem

Circuitos de segunda ordem são denominados dessa forma devido à presença de dois elementos que armazenam energia (em diversas configurações), cujas tensões e correntes são regidas por equações diferenciais de segunda ordem.

Em outras palavras, a dinâmica de circuitos de segunda ordem é descrita por equações diferenciais que envolvem a segunda derivada temporal de grandezas como tensão e corrente, refletindo como a energia é trocada entre campos elétricos e magnéticos nos capacitores e indutores presentes no circuito.

Estamos interessados em encontrar as EDOs de ordem 2 que descrevem a resposta destes circuitos ao estímulo natural e ao estímulo degrau, considerando sempre as configurações mistas dos elementos armazenadores de energia — circuitos RLC — compostos por resistores, capacitores e indutores.


---

## Introdução

<div class="regular">

- Nesta aula, a discussão da resposta natural e ao degrau está limitada a duas configurações: o circuito RLC em paralelo e o circuito RLC em série.

<div class="grid-25-25-25-25">

<div class="grid-element scriptsize">

A resposta natural de um circuito RLC em paralelo consiste em determinar a tensão criada nos ramos em paralelo pelo fornecimento de energia armazenada no indutor ou no capacitor ou em ambos, como na figura 1.

</div>
<div class="grid-element">
<figure>

<!-- _class: transparent -->
![grid-img](./img/circuito-rlc-paralelo-natural.png)

<figcaption class="center tiny">

Figura 1: Circuito que ilustra a resposta natural de um circuito \\(RLC\\) paralelo.

</figcaption>

</figure>
</div>

<div class="grid-element scriptsize">

Ao aplicar repentinamente uma fonte de corrente contínua (estímulo degrau) em um circuito \\(RLC\\) em paralelo, busca-se entender a tensão nos ramos paralelos, considerando a energia inicial no circuito em \\(t_{0}\\). A representação desse processo é mostrada na figura 2.

</div>

<div class="grid-emelent">
<figure>

<!-- _class: transparent -->
![grid-img](./img/circuito-rlc-paralelo-degrau.png)

<figcaption class="center tiny">

Figura 2: Circuito que ilustra a resposta ao degrau de um circuito \\(RLC\\) paralelo.

</figcaption>

</figure>
</div>

</div>

<div class="grid-25-25-25-25">

<div class="grid-element scriptsize">

A resposta natural de um circuito RLC em série consiste em determinar a corrente gerada nos elementos em série pela descarga (fornecimento) da energia armazenada no indutor, no capacitor ou em ambos, como na figura 3.

</div>
<div class="grid-element">
<figure>

<!-- _class: transparent -->
![grid-img](./img/circuito-rlc-serie-natural.png)

<figcaption class="center tiny">

Figura 3: Circuito que ilustra a resposta natural de um circuito \\(RLC\\) série.

</figcaption>

</figure>
</div>

<div class="grid-element scriptsize">

Ao aplicar repentinamente uma fonte de tensão contínua (estímulo degrau) em um circuito \\(RLC\\) em série, busca-se entender o comportamento da corrente do sistema — em todos os elementos do circuito, que estão em série — considerando a energia inicial do circuito em \\(t_{0}\\). A representação desse processo é mostrada na figura 4.

</div>

<div class="grid-emelent">
<figure>

<!-- _class: transparent -->
![grid-img](./img/circuito-rlc-serie-degrau.png)

<figcaption class="center tiny">

Figura 4: Circuito que ilustra a resposta ao degrau de um circuito \\(RLC\\) paralelo.

</figcaption>

</figure>
</div>

</div>

</div>


---

## Resposta Natural do Circuito RLC Paralelo

<div class="grid-66-33 regular">

<div class="grid-element">

- Na resposta natural, estamos interessados na tensão \\(v(t)\\) do circuito. Como todos os elementos estão em paralelo \\(C, L \text{ e } R\\) sabemos que eles possuem a mesma tensão, portanto, \\(v(t)\\) nossa grandeza de interesse é partilhada por eles.

<div class="grid-50-50">

<div class="grid-element footnotesize">

- Entretanto, \\(v(t)\\) ainda é desconhecida e por sabermos que o circuito \\(RLC\\) é um circuito de segunda ordem, devemos de alguma forma encontrar expressões que possuam derivadas de \\(v(t)\\) até a segunda ordem.

</div>

<div class="grid-element footnotesize">

- Pela lei de Ohm, bem como, pelas equações de capacitância e indutância (vistas na [aula cinco](https://diegoascanio.github.io/ace-aula-05)), podemos escrever as correntes de cada um destes elementos em função de \\(v(t)\\), nossa grandeza de interesse e até então, desconhecida.

</div>

</div>

</div>

<div class="grid-element">

<!-- _class: transparent -->
![grid-img](./img/circuito-rlc-paralelo-natural.png)

</div>

</div>

<div class="grid-25-25-25-25 small">

<div class="grid-element">

Em função de \\(v(t)\\):

\\[
\begin{align}
    I_{C}(t) &= C \frac{dv(t)}{dt} \\\\
    I_{R}(t) &= \frac{v(t)}{R} \\\\
    I_{L}(t) &= \frac{1}{L} \int v(t) dt + I_{L}(0)
\end{align}
\\]

</div>

<div class="grid-element scriptsize">

Pela Lei de Kirchoff das correntes nos nós:

\\[
\begin{align}
    &I_{C}(t) + I_{R}(t) + I_{L}(t) = 0 \therefore \\\\
    &C \frac{dv(t)}{dt} + \frac{v(t)}{R} + \frac{1}{L} \int v(t) dt + I_{L}(0) = 0
\end{align}
\\]


</div>

<div class="grid-element tiny">

Podemos derivar os dois lados da equação à esquerda em relação ao tempo \\(t\\):

\\[
\begin{align}
    \frac{d}{dt} &\left( C \frac{dv(t)}{dt} + \frac{v(t)}{R} \right. \\\\ 
    &\left. + \frac{1}{L} \int v(t) dt + I_{L}(0) \right) = 0 \therefore \\\\
    &C \frac{d^{2}v(t)}{dt^{2}} + \frac{1}{R} \frac{dv(t)}{dt} + \frac{1}{L} v(t) = 0
\end{align}
\\]

\\(I_{L}(0)\\) é constante, portanto, \\(\frac{d}{dt} I_{L}(0) = 0\\).

</div>

<div class="grid-element footnotesize">

Já encontramos a derivada de segunda ordem de \\(v(t)\\), como esperávamos, agora, multiplicamos a equação por \\(1 \over C\\) e obtemos:

\\[
\begin{align}
    &\frac{d^{2}v(t)}{dt^{2}} + \frac{1}{RC} \frac{dv(t)}{dt} + \frac{1}{LC} v(t) = 0
\end{align}
\\]

</div>

</div>
