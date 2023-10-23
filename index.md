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
