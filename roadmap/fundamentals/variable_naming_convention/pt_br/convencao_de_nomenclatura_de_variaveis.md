## Convenção de Nomenclatura de Variáveis

**Traduções**

- [EN-US](../variable_naming_convention.md)
- [PT-BR](./convencao_de_nomenclatura_de_variaveis.md)

## Navegação
<details>
<summary><b>Menu</b></summary>

- [Como Nomear Variáveis Corretamente](#como-nomear-variáveis-corretamente)
  - [Seja descritivo e significativo](#seja-descritivo-e-significativo)
  - [Use convenções de capitalização consistentes](#use-convenções-de-capitalização-consistentes)
  - [Evite nomes de uma letra (exceto em escopos limitados)](#evite-nomes-de-uma-letra-exceto-em-escopos-limitados)
  - [Não use abreviações, a menos que sejam bem conhecidas](#não-use-abreviações-a-menos-que-sejam-bem-conhecidas)
  - [Refletir o tipo de dado ou a intenção quando for útil](#refletir-o-tipo-de-dado-ou-a-intenção-quando-for-útil)
  - [Mantenha os nomes concisos, mas não crípticos](#mantenha-os-nomes-concisos-mas-não-crípticos)
  - [Use nomes positivos para booleanos](#use-nomes-positivos-para-booleanos)
  - [Evite palavras reservadas e nomes enganosos](#evite-palavras-reservadas-e-nomes-enganosos)
  - [Mantenha consistência em todo o código](#mantenha-consistência-em-todo-o-código)
  - [Nomeie variáveis pelo que elas representam, não pelo que fazem](#nomeie-variáveis-pelo-que-elas-representam-não-pelo-que-fazem)
  - [Evite nomes genéricos demais](#evite-nomes-genéricos-demais)
  - [Use terminologia específica do domínio](#use-terminologia-específica-do-domínio)
  - [Renomeie variáveis quando seu propósito mudar](#renomeie-variáveis-quando-seu-propósito-mudar)
  - [Priorize a legibilidade sobre preferência pessoal](#priorize-a-legibilidade-sobre-preferência-pessoal)
- [Créditos](#créditos)
</details>

<br />

# Como Nomear Variáveis Corretamente

## Seja descritivo e significativo

- Use nomes que expliquem claramente o propósito da variável (ex.: `nomeUsuario` em vez de `usr`).  

## Use convenções de capitalização consistentes

- `camelCase` para a maioria das variáveis (comum em JavaScript, Java, Python, C/C++).  
- `snake_case` para linguagens como Python, onde é idiomático.  
- `PascalCase` geralmente reservado para classes, não para variáveis.  

> A convenção pode mudar de acordo com os padrões do projeto.

## Evite nomes de uma letra (exceto em escopos limitados)

- Aceitável em loops (`i`, `j`, `k`...) ou contextos matemáticos, mas não para variáveis gerais.  

## Não use abreviações, a menos que sejam bem conhecidas

- Prefira `tamanhoMaximo` em vez de `tamMax`, a menos que a abreviação seja amplamente compreendida.  

## Refletir o tipo de dado ou a intenção quando for útil

- Use substantivos no plural para coleções: `usuarios`, `listaItens`.  
- Use prefixos booleanos como `esta`, `tem`, ou `pode`: `estaAtivo`, `temPermissao`.  

Evite codificar informações de tipo desnecessariamente:

- Não use prefixos como `strNome` ou `intContagem`, a menos que a linguagem ou o projeto exija.  

## Mantenha os nomes concisos, mas não crípticos

- Equilibre legibilidade e brevidade (`mensagemErro` é melhor que `mensagemErroDetalhadaParaEntradaDoUsuario`).  

## Use nomes positivos para booleanos

- Prefira `estaHabilitado` em vez de `naoDesabilitado` para reduzir esforço mental.  

## Evite palavras reservadas e nomes enganosos

- Não sobrescreva funções ou palavras-chave nativas, ex.: `lista`, `string`, `classe`.  

## Mantenha consistência em todo o código

- Escolha um estilo de nomenclatura e aplique em todo o projeto para melhorar a legibilidade.  

## Nomeie variáveis pelo que elas representam, não pelo que fazem

- Foque no conceito `idadeUsuario` em vez do cálculo `anoAtualMenosAnoNascimento`.  

## Evite nomes genéricos demais

- Nomes como `dados`, `valor` ou `temp` devem ser usados apenas quando o significado for realmente óbvio.  

## Use terminologia específica do domínio

- Alinhe os nomes das variáveis com o negócio ou domínio do problema para melhorar a clareza.  

## Renomeie variáveis quando seu propósito mudar

- Se uma variável evoluir, atualize seu nome para refletir sua nova responsabilidade.  

## Priorize a legibilidade sobre preferência pessoal

- Escolha nomes que façam sentido para toda a equipe, não apenas para o autor.  

<br />

# Créditos

| [<img src="https://github.com/sdkitagawa.png?size=50" width=50><br /><sub>@sdkitagawa</sub>](https://github.com/sdkitagawa) |
| :---: |
