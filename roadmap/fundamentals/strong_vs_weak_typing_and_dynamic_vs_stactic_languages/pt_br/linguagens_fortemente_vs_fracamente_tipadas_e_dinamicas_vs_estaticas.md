## Tipagens e Tipos de Linguagens

**Translations**

- [EN-US](../strong_vs_weak_typing_and_dynamic_vs_stactic_languages.md)
- [PT-BR](./linguagens_fortemente_vs_fracamente_tipadas_e_dinamicas_vs_estaticas.md)

## Navigation
<details>
<summary><b>Menu</b></summary>

- [Introdução](#introdução)
- [O que é tipagem?](#o-que-é-tipagem)
- [Tipagem em Partes](#tipagem-em-partes)
    - [Tipagem Forte](#tipagem-forte)
    - [Tipagem Fraca](#tipagem-fraca)
    - [Linguagens Estáticas](#linguagens-estáticas)
    - [Linguagens Dinâmicas](#linguagens-dinâmicas)
- [Vínculos e Diferenças](#vínculos-e-diferenças)
    - [Tipagem Estática e Forte](#tipagem-estática-e-forte)
    - [Tipagem Estática e Fraca](#tipagem-estática-e-fraca)
    - [Tipagem Dinâmica e Forte](#tipagem-dinâmica-e-forte)
    - [Tipagem Dinâmica e Fraca](#tipagem-dinâmica-e-fraca)
- [Linguagens e seus Tipos](#linguagens-e-seus-tipos)
- [Créditos](#créditos)
</details>

<br />

# Introdução
Quando se está estudando programação e desenvolvimento é inevitável que cedo ou tarde você irá se deparar com termos como tipagem "**forte**", "**fraca**" e linguagem "**estática**" ou "**dinâmica**". E você encontrará uma série de discussões ao redor disso sobre qual linguagem é o que é, e por quais motivos.

Nesta aula iremos desvendar os mistérios por trás desse tema complicado e tão discutido.
<br /><br />

# O que é tipagem?
Tipagem é o que define se a sua linguagem vai ser mais lenta, dinâmica e com menor barreira de entrada para se aprender e trabalhar, ou se vai ser mais rápida, estática e com uma maior barreira de entrada para se aprender e trabalhar.

Acredite eu sei, há um dilema aqui, afinal, porque passar mais tempo estudando uma linguagem de programação complexa para entrar no mercado, quando na verdade estudando menos de uma linguagem de programação mais simples eu posso aprender a programar mais rápido e entrar no mercado o quanto antes?

Por mais que possa ser tentador pensar dessa maneira, meu trabalho como um bom professor e mentor é abrir os seus olhos o quanto antes para a realidade e esclarecer o quanto antes que quando falamos de tipagem nem sempre se trata da linguagem com menor barreira de entrada e menor complexidade no aprendizado ou o oposto.

Quando falamos de tipagem temos que levar em consideração uma série de fatores, tais como:

- O quanto você realmente vai estar aprendendo sobre os fundamentos essenciais para entender de fato o que está fazendo, como, o porque as coisas acontecem da maneira que acontecem, quais são as origens das tecnologias que temos disponíveis desde sempre;

- Se vale a pena focar em linguagens como **JavaScript**, **Perl** e **PHP** que por possuírem uma **tipagem fraca** te proporcionam _mais agilidade_ devido a _não necessidade de tipagem dos dados_, maior liberdade para desenvolver algo sem se preocupar demais com o _design do sistema_, ter uma _sintaxe mais simples_, _menor curva de aprendizado_ para novatos e etc. Sendo que mais tarde _perderá mais tempo_ se preocupando com uma maior quantidade de _bugs que apareceram em tempo de execução_ exatamente devido a falta de tipagem forte, te causando problemas futuros em aplicações que crescem e escalam mais do que o esperado. Forçando você e a sua equipe a colocarem um esforço enorme na criação de [testes unitários (Unit Tests)](https://aws.amazon.com/what-is/unit-testing/), [linters](https://www.testim.io/blog/what-is-a-linter-heres-a-definition-and-quick-start-guide/), [CI/CD (Continuous Integration/Continuous Delivery)](https://about.gitlab.com/topics/ci-cd/) e etc;

- Talvez valha a pena focar em linguagens como **C#** e **Java** que por possuírem uma **tipagem forte** te proporcionam _maior segurança_ no desenvolvimento, já que _menos bugs ocorrem em tempo de execução_, você também presta _maior atenção no design do seu sistema_ desde os primeiros estágios de desenvolvimento. Sendo que no final das contas você tem uma maior curva de aprendizado para novatos, e te faz _perder agilidade e tempo_ tendo que constantemente inferir tipos corretamente, entender a complexidade dos tipos e trabalhar com muito [código boiler plate](https://aws.amazon.com/what-is/boilerplate-code/#:~:text=Boilerplate%20code%20is%20computer%20language,minimal%20changes%20for%20different%20situations.);

Dito tudo isto, sem mais enrolação, vamos as explicações mais diretas.
<br /><br />

# Tipagem em Partes
### Tipagem Forte
- Variáveis na grande maioria dos casos não podem ser **Nulas**;
- Variáveis devem possuir um tipo;
- Variáveis devem ser inicializadas;
- Variáveis não podem ter seu tipo alterado após terem sido declaradas.
<br /><br />

### Tipagem Fraca
- Variáveis podem ser **Nulas**;
- Variáveis não necessitam de um tipo, pois, a própria linguagem determina um tipo com base no dado armazenado na mesma;
- Variáveis não necessariamente precisam ser inicializadas (mas podem, se necessário);
- Variáveis podem ter seu tipo alterado mesmo após terem sido declaradas.
<br /><br />

### Linguagens Estáticas

Linguagens estáticas não permitem que você altere o tipo da variável depois de declarada.

- Anti-Dinamismo;
  - A linguagem é compilada;
  - Você tem feedback sobre o seu código em tempo real através da sua IDE (dentro do seu editor de código);
  - Existe uma melhor performance em tempo de execução;
  - Fornece maior segurança;
  - Erros são detectados mais rapidamente (_redundante com o ponto 2, mas ainda assim mencionável_);
  - Processo mais demorado para prototipação;
  - São as melhores para se desenvolver um jogo, aplicações relacionadas a segurança, sistemas embarcados (sistemas normalmente desenvolvidos para máquinas e robôs), sistemas operacionais, firmwares (micro-sistemas operacionais desenvolvidos normalmente para consoles portáteis, modems, roteadores, aparelhos de transmissão de serviço de TV á cabo).
<br /><br />

### Linguagens Dinâmicas

Linguagens dinâmicas estão ligadas a habilidade de permitir que a mesma variável possa receber valores de tipos diferentes ao longo da execução do código.

- Dinamismo;
  - A linguagem é interpretada;
  - Você não tem feedback sobre o seu código em tempo real através da sua IDE (dentro do seu editor de código) sem o uso de linters;
  - Pior performance e tempo de execução;
  - Menor segurança;
  - Processo mais rápido para prototipação;
  - São as melhores para sistemas backend para sites, sistemas backend para aplicativos, sistemas de redes neurais (inteligência artificial), renderização de vídeos e imagens através de código, cálculos quânticos / complexos (sistemas de clima, tempo e outras utilidades envolvendo a física)
<br /><br />

# Vínculos e Diferenças
### Tipagem Estática e Forte
Linguagens de tipagem estática e forte te entregam os seguintes recursos, como:

- Verificação de tipos em tempo de compilação;
- Inferência de tipos explícita;
  - Forçando o desenvolvedor a sempre ter que dizer qual é o tipo de variável;
- Menos conversões implícitas.
  - Quando você está trabalhando com dois tipos de dados incompatíveis, como uma `string` e um `inteiro`, você não consegue executar uma soma com isto, logo, você não pode simplesmente converter um valor no outro, sendo necessário o uso de Casts e Parsers para transformar os tipos.
<br /><br />

### Tipagem Estática e Fraca
Linguagens de tipagem estática e fraca por outro lado entregam:

- Verificação de tipos em tempo de compilação;
- Conversão de tipos implícitas
  - Você pode fazer conversões de tipos de dados sem muitas dificuldades.
<br /><br />

### Tipagem Dinâmica e Forte
Linguagens de tipagem dinâmica e forte entregam:

- Não permissão de operações entre tipos diferentes sem conversão explícita;
- Não permissão de operações automáticas ("mágicas") entre tipos incompatíveis.
<br /><br />

### Tipagem Dinâmica e Fraca
Linguagens de tipagem estática e fraca entregam:

- Flexibilidade de tipos;
  - Por exemplo, somar um tipo `inteiro` com uma `string` e ter como resultado disso um `inteiro`.
- Conversões de tipos automáticas ("mágicas").
<br /><br />

# Linguagens e seus Tipos
Modo de leitura da tabela:
- Leia começando pelo **eixo Y** (de cima para baixo) de forma vertical;
- Em seguida, leia o **eixo X** (da esquerda para a direita) de forma horizontal.

| **Intensidade** | **Estática** | **Dinâmica** |
|:--:|:--:|:--:|
| **Forte** | C#, Dart, Delphi, F#, Haskell, Java, Kotlin, Pascal, Rust, Scala, Swift | Clojure, Erlang, Groovy, Lua, Python, Ruby, TypeScript |
| **Fraca** | C, C++, C--, C*, COBOL | CoreSE, JavaScript, Perl, PHP, Visual Basic |

# Créditos

| [<img src="https://github.com/sdkitagawa.png?size=50" width=50><br /><sub>@sdkitagawa</sub>](https://github.com/sdkitagawa) |
| :---: |
