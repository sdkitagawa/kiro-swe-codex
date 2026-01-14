## Google Dorking/Hacking

**Traduções**

- [EN-US](../google_dorking_hacking.md)
- [PT-BR](./google_dorking_hacking.md)

## Navegação
<details>
<summary><b>Menu</b></summary>

- [O que é Google Dorking/Hacking](#o-que-é-google-dorkinghacking)
- [Para que serve?](#para-que-serve)
- [Quais são os filtros?](#quais-são-os-filtros)
- [Como funciona?](#como-funciona)
- [Exercícios](#exercícios)
- [Créditos](#créditos)
</details>

<br />

# O que é Google Dorking/Hacking

Google Dorking/Hacking é basicamente uma técnica que consiste em comandos, ou operadores, que permitem modificar os resultados de busca de acordo com o tipo de dado buscado.
<br /><br />

# Para que serve?

Google Dorking/Hacking tem como objetivo atuar como um filtro detalhado de pesquisa que quando usando o [Google](https://www.google.com/), a própria ferramenta não trás acesso as esses recursos de forma fácil através da sua interface.

Através desta técnica você consegue encontrar coisas específicas em partes diversas de um resultado de pesquisa do Google.

Observando a imagem abaixo, observe as propriedades que um resultado de uma pesquisa no Google pode trazer.
<br /><br />
<center>
        <img src="../assets/google_search_assets.png" alt="Propriedades de uma pesquisa feita no Google" width="700" align="center" />
</center>
<br /><br />

# Quais são os filtros?
Existem diversos filtros para executarmos as técnicas de Google Dorking/Hacking, então antes de sairmos usando-os, vamos entender quais são os filtros e como eles funcionam.

| Parâmetros ou Operadores | Valores | Como usar | Detalhes do Uso | Efeito |
|--------------------------|--------|-----------|----------------|--------|
**Palavra 1 Palavra 2 Palavra 3** | **Casa Branca Presidente** | `Coisa Sujeito Objeto` | Insira as palavras que deseja buscar uma do lado da outra intercalando com espaços vazios | Tentará encontrar nos resultados das pesquisas as três palavras **SEPARADAMENTE** em um mesmo resultado de pesquisa |
**filetype**, **ext** | **filetype:PDF** | `filetype:Extensão` ou `ext:Extensão` | Use o operador e aponte uma extensão | Tentará encontrar arquivos com o tipo apontado. Cheque [este link](https://developers.google.com/search/docs/crawling-indexing/indexable-file-types?hl=en&visit_id=638010780742925546-492926684&rd=1) para saber quais extensões de arquivo o Google pode indexar (armazenar) |
**intitle**, **allintitle** | **intitle:Nintendo** | `intitle:Coisa` ou `allintitle:Coisa` | Use o operador e em seguida passe como parâmetro algo que você deseja encontrar em títulos de páginas | Tentará encontrar páginas que tenham seu título igual ao texto passado como parâmetro |
**inurl** | **inurl:contato.php** | `inurl:Algum Elemento Dentro do Link` | Use o operador e em seguida passe algum texto que deseja encontrar presente no endereço URL (link) | Tentará trazer qualquer página que contenha o que você passou como parâmetro dentro do URL (link) |
**allinurl** | **allinurl:Jogos Baratos** | `allinurl:O que você quer buscar` | Use o operador e em seguida digite o que deseja encontrar | Tentará trazer qualquer página que contenha as palavras que tenham sido passadas após os dois pontos em um endereço URL (link) |
**intext** | **intext:Gosta de água** | `intext:Texto Aqui` | Use o operador e dentro das aspas escreva exatamente o texto que deseja encontrar | Tentará encontrar exatamente aquele texto em meio ao resto do texto |
**allintext** | **allintext:Gosto de suco** | `allintext:Texto aqui` | Use o operador e após os dois pontos escreva exatamente o texto que deseja encontrar em toda a consulta (não somente em texto) | Trará como resultado da pesquisa o texto buscado não somente na parte de descrição, mas também em títulos e outros (hoje este filtro é praticamente inútil) |
**site** | **https://facebook.com** | `Mark Zuckerberg site:https://facebook.com` | Use o operador e em seguida aponte o site onde deseja encontrar informações | Tentará encontrar qualquer coisa pesquisada dentro do site especificado |
**stocks** | **stocks:Amazon** | `stocks:Nome da Empresa` | Use o operador e em seguida aponte o nome da empresa que deseja checar atividades financeiras | Encontrará resultados das atividades financeiras públicas da empresa |
**in, to** | **10 usd in brl** | `Número, Sigla da Moeda de Origem in Sigla da Moeda de Destino` ou `Número, Sigla da Moeda de Origem to Sigla da Moeda de Destino` | Passe um valor numérico, use os operadores **in**/**to** entre as siglas das moedas | Fará a conversão de uma moeda em outra. Para saber as siglas das moedas use [este link](https://pt.iban.com/currency-codes) |
**movie** | **movie:Kung Fu Panda** | `movie:Nome do Filme` | Use o operador e aponte o nome do filme que deseja encontrar | Encontrará informações sobre o filme pesquisado. Recomenda-se colocar o nome do filme entre aspas duplas |
**source** | **source:CNN** | `source:Nome da Empresa` | Use o operador e em seguida o nome da empresa, site, revista ou blog | Encontrará relatórios de pesquisas relacionados ao que procurou, com fontes do Google News |
**cache** | **cache:msn.com** | `cache:Endereço do Site` | Use o operador seguido do endereço do site | Encontrará a última versão armazenada na memória cache do Google do site |
**location**, **loc** | **location:NY Pontos Turísticos** | `location:LOCAL Busca de Local` ou `loc:LOCAL Busca de Local` | Insira uma sigla do local desejado e depois a informação que deseja buscar | Trará resultados relacionados à informação apenas no local especificado |
**map** | **map:São Paulo** | `map:Nome da Cidade` | Insira o operador seguido do **nome da cidade** | Retorna um mapa da cidade apontada |
**weather** | **weather:São Paulo** | `weather:Nome da Cidade` | Insira o operador seguido do **nome da cidade** | Retorna informações do clima da cidade |
**link** | **link:facebook.com** | `link:Endereço do Site` | Insira o operador seguido do link do site desejado | Trará páginas relacionadas ao domínio especificado |
**related** | **related:harvard.edu** | `related:Endereço do Site` | Insira o operador seguido do endereço do site | Retorna sites relacionados ao site especificado |
**info**, **id** | **info:"Twitter"** | `info:"Nome do Site"` ou `id:"Nome do Site"` | Insira o operador seguido do nome do site | Retorna páginas com informações sobre o site especificado |
**AND**, **&** | **Jennifer Lopez AND Ja Rule** | `Coisa 1 AND Coisa 2` ou `Coisa 1 & Coisa 2` | Insira um sujeito/alvo e use **AND** para combinar com outro alvo | Tentará encontrar **Coisa 1 E Coisa 2** nos resultados |
**OR** | **Alyne OR Allyne** | `Coisa 1 OR Coisa 2` | Insira o sujeito/alvo e use **OR** para combinar | Tentará encontrar **Coisa 1 OU Coisa 2** nos resultados |
**+** | **Velozes e Furiosos +Tokyo** | `Coisa +Sujeito` ou `Sujeito +Coisa` ou `10 + 10` | Insira um sujeito/alvo/objeto e use **+** para adicionar outro | Tentará encontrar **Coisa +Sujeito** ou somar números |
**-** | **Mark Zuckerberg -Facebook** | `Sujeito -Coisa` ou `Coisa -Sujeito` | Insira um sujeito/alvo/objeto e use **-** para subtrair outro | Tentará encontrar **Coisa -Sujeito** ou subtrair números |
**\*** | **mac * OS** | `Palavra 1 * Palavra 2` | Insira duas palavras separadas por `*` | Tentará encontrar **Palavra 1** e **Palavra 2** com no máximo uma palavra entre elas; também multiplica números |
**/** | **14 / 2** | `Número 1 / Número 2` | Insira um número, use **/** e outro número | Fará a divisão do número 1 pelo número 2 |
**sin, cos, tan** | **sin(pi/6)** ou **sin 30 degrees** | `Operação(valor 1, operador, valor 2)` ou `Operador, valor, ângulo` | Insira números e operadores | Calcula Seno, Cosseno ou Tangente |
**sqrt(N)** | **sqrt(4)** | `RaizQuadra(valor)` | Insira a palavra-chave **sqrt** com um número | Retorna a raiz quadrada do número |
**% of** | **17% of 500** | `Valor% of ValorTotal` | Insira valor, `%`, **of**, e valor total | Retorna a porcentagem do valor especificado |
**~** | **Angelina Jolie ~linda amigável** | `Sujeito/alvo/coisa ~Predicado1 Predicado2` | Insira o sujeito/alvo/coisa e qualidades para buscar sinônimos | Retorna resultados com sinônimos das palavras após **~** |
**""** | **"Exatamente isto"** | `"Texto exato"` | Insira palavras entre aspas duplas | Buscará exatamente o que está entre aspas |
**()** | `(Video games PlayStation) AND (Angelina Jolie)` | `(BuscaPrimária) OutroOperador (BuscaSecundária)` | Insira buscas entre parênteses e combine com operadores | Trará resultados mais claros e organizados |
**X..Y** | **Resident Evil Games 2010..2024** | `AnoInicial..AnoFinal` | Insira a pesquisa seguida do ano inicial e final separados por dois pontos | Filtra resultados entre os anos especificados |
**define** | **define:Crux** | `define:Palavra` | Insira **define:** seguido da palavra | Retorna definições da palavra |
**@** | **@youtube Astro Política** | `@social Busca` | Insira operador, rede social, e termo de busca | Retorna resultados relacionados à rede social |
**$**, **€**, **£**, **¥**, **₩**, **₹** | **PlayStation 2 ¥** | `NomeDoProduto $` | Insira nome do produto e símbolo da moeda | Retorna preços do produto na moeda especificada |
**filter** | **Olho de Horus filter:1** | `Sujeito/Coisa filter:0` ou `filter:1` | Insira pesquisa e **filter:** com 0 ou 1 | Inclui/exclui resultados duplicados (`0` = duplicatas, `1` = sem duplicatas) |
**AROUND()** | **AROUND(14) Final Fantasy** | `AROUND(N) Busca` | Insira **AROUND** com número entre parênteses | Localiza termos separados por até N palavras |
**timer** | **timer for 30 minutes** | `time for N hours/minutes/seconds/milliseconds` | Insira **timer for** + número + unidade | Cria contagem regressiva |
**flip a coin** | **flip a coin** | `flip a coin` | Copie na barra de pesquisa | Joga uma moeda |
**roll a dice** | **roll a dice** | `roll a dice` | Copie na barra de pesquisa | Rola um dado |
**show a random number** | **show a random number from 10 to 120** | `show a random number from N1 to N2` | Copie na barra de pesquisa | Mostra número aleatório entre N1 e N2 |
**as_epq** | **O ontem é história, o amanhã é um mistério, mas o hoje é uma dádiva. É por isso que se chama presente. as_epq** | `Frase Desejada as_epq` | Insira frase ou sentença e use **as_epq** | Retorna exatamente a frase antes do parâmetro |
**as_filetype** | **O Código da Vinci as_filetype:PDF** | `Busca as_filetype:Extensão` | Use **as_filetype** e extensão | Funciona como **filetype**, pode ser combinado com **as_ft** |
**as_ft** | **O Código da Vinci as_filetype:PDF as_ft:i** | `Busca as_filetype:Extensão as_ft:i/e` | Use **as_ft** após **as_filetype** | Inclui/exclui arquivos por extensão (`i` = incluir, `e` = excluir) |
**as_occt** | **Goécia as_occt:body** | `Busca as_occt:body/title/url/links` | Insira operador **as_occt** e escolha área | Pesquisa em partes específicas do site: **any, title, body, url, links** |
**as_sitesearch** | **as_sitesearch:facebook.com** | `as_sitesearch:Domínio/Site` | Insira operador e domínio/site | Igual ao operador **site**, mas com filtro adicional **as_dt** |
**as_dt** | **Serviço de Streaming as_sitesearch:netflix.com as_dt:e** | `as_sitesearch:Domínio as_dt:i/e` | Use **as_sitesearch** + domínio + **as_dt** | Inclui/exclui domínios ou sites (`i` = incluir, `e` = excluir) |
**as_qdr** | **as_qdr:m3** | `as_qdr:Quantidade` | Use **as_qdr** com meses ou anos abreviados | Retorna páginas atualizadas no período (`M` = mês, `Y` = ano) |

<br /><br />

# Como funciona?

Google Dorking/Hacking funciona através de filtros de pesquisa que são dados como comandos, por exemplo, vamos imaginar um cenário hipotético onde você deseja encontrar informações sobre `Larry Page` e `Sergey Brin` os fundadores do Google, mas você quer encontrar informações sobre eles em um site específico, o site que vamos usar de exemplo é o Futurism, que é uma companhia de mídia digital que trás notícias constantes de ciência e tecnologia.

Então, vamos pensar da seguinte forma:

**1 -** Vamos identificar os nossos sujeitos ou "alvos";

**2 -** Vamos pensar onde desejamos encontrar as informações sobre nossos sujeitos/alvos;

**3 -** Vamos montar uma sentença lógica através de comandos lógicos e semelhantes aos de programação, usando os filtros de Google Dorking/Hacking;.

**Nota:**
> Tendo esses passos em mente, irei exemplificar como podemos alcançar o que desejamos

<br />

**Pergunta 1:** Quem é/são meu(s) sujeito(s)/alvo(s)?<br />
**Resposta 1:** Sergey Brin e Larry Page (juntos, nem somente um e nem somente o outro);

**Pergunta 2:** Onde eu desejo pesquisar sobre meu(s) sujeito(s)/alvo(s)?<br />
**Resposta 2:** No site `https://futurism.com/`;

**Pergunta 3:** Como montar isso logicamente usando os filtros de Google Dorking/Hacking.<br />
**Resposta 3:** "sergey brin" AND "larry page" site:https://futurism.com/
<br /><br /><br /><br />

# Exercícios
**Todos os exercícios abaixo devem ser feitos utilizando a ferramenta Google de pesquisa**.

**1** - Procure por informações sobre a série iCarly de forma filtrada, encontrando resultados que venham somente da distribuidora oficial da série (Paramount Plus).
**R:** 

**2** - Usando a aba de imagens do Google, busque por imagens do seriado Hannah Montana que estejam no formato `PNG`:
**R:** 

**3** - Busque pelo usuário "iruletheworldmo" dentro da plataforma Twitter sem usar o operador `site`.
**R:** 

**4** - Busque pela definição das palavras a seguir "Noctis", "Lucis", "Caelum" e "Nox"
**R:** 

**5** - Cheque como está o resumo financeiro das ações das empresas NVIDIA, AMD, Intel e Microsoft.
**R:** 

**6** - Procure pelo filme "O Código da Vinci"
**R:** 

**7** - Procure por fontes de informações com este título de uma notícia "Microsoft 365 anti-phishing feature can be bypassed with CSS" na plataforma BleepingComputer sem usar o operador `site`.
**R:** 

**8** - Procure pelo preço atual do iPhone 15 em Euro, Yen e Dólar.
**R:** 

**9** - Tente buscar no Cache do Google a página "narutoproject.com".
**R:** 

**10** - Procure por páginas vinculadas ao domínio `thatsthefinger.com`.
**R:** 

**11** - Procure por páginas relacionadas ao domínio do Facebook (`facebook.com`).
**R:** 

**12** - Procure pelo mapa de Santa Catarina.
**R:** 

**13** - Procure pelo clima de Toyokawa.
**R:** 

**14** - Procure por coisas para fazer em São Paulo.
**R:** 

**15** - Procure por informações sobre a empresa `GRAVITY Interactive` dentro de algum site.
**R:** 

**16** - Procure por páginas que contenham a palavra `Ted's caving journal` em seu título.
**R:** 

**17** - Procure por páginas que possuam uma página chamada de `contato` com a extensão `php` em seu site.
**R:** 

**18** - Procure páginas que contenham em seu texto a seguinte frase `entre em contato`.
**R:** 

**19** - Procure de forma geral (em qualquer parte de um resultado de pesquisa, podendo ser título, descrição e etc) por EXATAMENTE está frase `Nunca discuta com um ignorante. Ele te rebaixará até o nível dele e te vencerá por experiência.`.
**R:** 

**20** - Procure por Jéssica Canedo, queremos resultados relacionados a Banca Digital ou Mynd e reporte o que encontrou.
**R:** 

**21** - Procure por processadores da Intel que não seja da geração i3 e i7.
**R:** 

**22** - Faça uma busca por tudo que puder sobre A858 entre 2011 até 2024.
**R:** 

**23** - Execute operações matemáticas de `soma`, `subtração`, `multiplicação`, `divisão` e `raiz quadrada` utilizando o Google.
**R:** 

**24** - Converta R$ 300 (reais) em $ (dólar americano).
**R:** 

**25** - Procure pelo seu nome e procure por documentos na extensão `PDF`, `DOCX`, `DOC`, `PPTX`, `PPT`, `XLS`, `XLSX` e `TXT`.
**R:** 

**26** - Procure pelo filme `Efeito Borboleta`.
**R:** 

# Créditos

| [<img src="https://github.com/sdkitagawa.png?size=50" width=50><br /><sub>@sdkitagawa</sub>](https://github.com/sdkitagawa) |
| :---: |
