## Linguagens Compiladas vs. Linguagens Interpretadas

**Traduções**

- [EN-US](../difference_compiled_vs_interpreted_languages.md)
- [PT-BR](./diferenca_linguagens_compiladas_vs_interpretadas.md)

## Navegação
<details>
<summary><b>Menu</b></summary>

- [Introdução](#introdução)
- [Tipos de Linguagem de Programação](#tipos-de-linguagem-de-programação)
- [Dividindo o Problema em Partes](#dividindo-o-problema-em-partes)
  - [Parte 1](#parte-1)
  - [Parte 2](#parte-2)
  - [Conclusão do Problema](#conclusão-do-problema)
- [Como funcionam](#como-funcionam)
    - [Linguagens Compiladas](#linguagens-compiladas)
    - [Linguagens Interpretadas](#linguagens-interpretadas)
- [Tabela Comparativa](#tabela-comparativa)
- [Créditos](#créditos)
</details>

<br />

# Introdução

No universo dos computadores todas as linguagens de programação são simples instruções que cedo ou tarde se tornam Hexadecimais ou Binários e veremos isso mais a fundo em breve. Talvez você esteja se perguntando, onde você quer chegar com isso?

Na verdade é bem simples, nesta aula você aprenderá a diferença entre as linguagens de programação compiladas e as linguagens de programação interpretadas.

# Tipos de Linguagem de Programação

As linguagens de programação até o momento são dividas em 2 tipos:

- Linguagens Compiladas
- Linguagens Interpretadas

Não se desespere, veremos em detalhes as diferenças entre elas com alguns exemplos vistos de fora.

Como tudo em um computador, desde o hardware até o funcionamento das tecnologias sempre partem de algo que o ser humano tem um alto conhecimento e experiência a respeito. Com as linguagens de programação não é muito diferente.

# Dividindo o Problema em Partes
## Parte 1

**1.** Imaginemos o cenário hipotético onde você tem um manual para instalação de uma nova ferramenta que você começará a utilizar no seu dia-a-dia no trabalho;<br />
**2.** Você está no Japão, e nesse exemplo hipotético você não fala, não lê e não escreve em Japonês;<br />
**3.** Você precisa ser capaz de efetuar a instalação do software corretamente;<br />
**4.** Você não vive em um mundo tecnológico com smartphones, torres de celulares com suporte a tecnologias como 3G, 4G, 5G ou quaisquer outros recursos de internet com Wi-Fi, Hot spot e etc.
<br /><br />

## Parte 2

Sabendo que este é o cenário te restam algumas poucas alternativas, que são:

**A)** Se houver um setor responsável por tradução dentro da empresa, eles se responsabilizaram por traduzirem o manual de instalação do Japonês para o seu idioma nativo;<br />
**B)** Se você possuir um amigo que fale e leia Japonês ele pode sentar ao seu lado durante o processo de instalação e fazer a tradução linha por linha em tempo real para você.
<br /><br />

## Conclusão do Problema

Na opção **A** você tem alguém que traduz tudo para o seu idioma nativo para que ai sim as coisas possam ser executadas, e isto é equivalente a uma **Linguagem Compilada**.

Por outro lado, na opção **B** você tem uma pessoa que interpreta tudo que está escrito, e então, traduz as coisas etapa por etapa para você, e isto é equivalente a uma **Linguagem Interpretada**.
<br /><br />

# Como funcionam
### Linguagens Compiladas

As linguagens compiladas funcionam convertendo as instruções em inglês que são digitadas por Programadores, Desenvolvedores e Engenheiros de Software em linguagem de máquina, também chamado de **Linguagem Binária** ou **Sistema Binário**, essa, não por acaso é a lingua que o seu processador (CPU) usa para se comunicar com todas as partes (peças de hardware) e sistemas dentro do seu computador.

Uma outra característica das linguagens compiladas é que justamente por converter instruções de textos em inglês em código que seja compreensível e legível para a máquina essas linguagens necessitam de uma etapa que chamamos de **Building** (montagem ou construção), que seria literalmente para que o **Compilador** leia todas as suas instruções em Inglês e depois as converta em números binários para o processador. Elas também dão ao desenvolvedor mais controle sobre alguns aspectos do hardware, como o gerenciamento da memória e o uso da CPU.

Durante essa etapa de Building as suas instruções escritas em Inglês são convertidas em um arquivo que chamamos de `Binaries` (Binários) e que mais tarde será compreendido pelo computador com maior facilidade quando houver a necessidade de executar aquele programa, afinal, o programa já terá sido convertido em algo que está na própria língua do computador. Normalmente o seu código é convertido em arquivos com extensões de arquivo `.exe` (Windows), `.app` (macOS), `dll` (Windows), `kext` (macOS) dentre outros.

E justamente também devido a etapa de Building, linguagens tendem a ser mais rápidas para desenvolvimento de aplicações muito pesadas, tais como, jogos, sistemas operacionais e outras aplicações de alto desempenho.
<br /><br />

### Linguagens Interpretadas

As linguagens interpretadas por outro lado em sua maioria funcionam através de uma tecnologia que chamamos de [JIT Compilation](https://en.wikipedia.org/wiki/Just-in-time_compilation) (Just In time Compilation ou Compilação na Hora Certa) ou Compilação Dinâmica que resumidamente é um método para aprimorar a performance de linguagens interpretadas fazendo com que durante a execução, o programa possa ser compilado em código nativo para aprimorar a sua performance e tempo de resposta.

Caso ainda não tenha ficado clara a grande diferença entre as linguagens compiladas e interpretadas aqui vai uma grande dica. As linguagens interpretadas passam pelo código de um programa linha por linha executando cada comando. Um detalhe importante é que uma linguagem em seu todo não necessariamente é 100% interpretada, existem casos como a linguagem Python, por exemplo, que é apesar de ser considerada uma linguagem interpretada tem C atuando na sua camada mais baixa para compilar certas informações rapidamente.
<br /><br />
<br /><br />

# Tabela Comparativa
<br /><br />

| **Quesitos** | **Linguagens Compiladas** | **Linguagens Interpretadas** |
|:--:|:--:|:--:|
| **Building** | Necessita de uma etapa de *building* (montagem/construção). O compilador lê todo o código, transforma em um arquivo binário e o envia para a CPU executar. | Não necessariamente necessita de *building* para todas as funcionalidades. Trechos de código são compilados dinamicamente por um interpretador e enviados para a CPU executar. |
| **Funcionamento** | Depende de um compilador para compilar seu código. | Na maioria dos casos, não depende de um compilador para executar o código. |
| **Análise Sintática** | Analisa erros no código previamente e impede a geração do código de máquina (binário) caso haja erros. | Não analisa erros previamente; executa o código e alerta sobre erros durante a execução. |
| **Velocidade de Desempenho** | Geralmente possuem melhor desempenho e maior velocidade por se comunicarem diretamente com a máquina após a conversão para binário. | Possuem menor desempenho, porém permitem modificação do código em tempo de execução. Há exceções, como quando o Python utiliza código em C para otimizações. |
| **Capacidade de Manipulação de Memória** | Maior capacidade de manipulação de memória, com uso de ponteiros, aritmética de ponteiros e alocação/liberação manual. | Menor flexibilidade na manipulação direta de memória. |
| **Linguagens** | Assembly, B, Basic, C, C++, C#, Delphi, Fortran, Go, Java, Pascal, Rust, Visual Basic | Bash, CoreSE, JavaScript, Lua, Perl, PHP, Python, R, Ruby |
| **Uso** | Sistemas Operacionais, Jogos, Sistemas Embarcados, Nuvem, IoT | Ciência de Dados, Aprendizado de Máquina, Aplicativos, Análise de Dados |

<br />

# Créditos

| [<img src="https://github.com/sdkitagawa.png?size=50" width=50><br /><sub>@sdkitagawa</sub>](https://github.com/sdkitagawa) |
| :---: |
