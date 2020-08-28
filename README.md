# Seletores CSS

- TAG - O seletor de tag é o mais simples de todos, basta informar o nome da tag por exemplo p, e todas as tags p existentes no documento receberão a formatação indicada.

- ID - O seletor para id é mais específico do que o de tags, formata somente a tag que possui o id especificado, para indicar
que o seletor será para um id basta anteceder o nome do id com o caractere hash “#”.

- CLASS -Este selector formata todos os elementos que usam a classe indicada, desta maneira podemos ter várias tags p

por exemplo, somente receberão a formatação aquelas que tiverem o atributo class com o nome da classe
configurada, para identificar este seletor, basta usar um ponto “.” antes do nome da classe.

Podemos indicar mais de um seletor para receber um conjunto de formatações CSS, basta indicar estes seletores 
separados por vírgulas

```

Seletor CSS                 |Exemplo                      |Descrição
----------------------------|-----------------------------|-----------
.classe                     |.intro                       |Seleciona todos os elementos que usam a classe intro / class="intro"
#id                         |#primeiroNome                |Seleciona o elemento com o id primeiroNome / id="primeiroNome"
*                           |*                            |Seleciona todos os elementos
elemento                    |p                            |Seleciona todos os elementos com a tag <p>
elemento,elemento           |div, p                       |Seleciona todos os elementos <div> e <p>
elemento elemento           |div p                        |Seleciona todos os elementos <p> que estão dentro de elementos <div>
elemento>elemento           |div > p                      |Seleciona todos os elementos <p> onde o pai seja um elemento <div>
elemento+elemento           |div + p                      |Seleciona todos os elementos <p> que estão posicionados imediatamente após o elemento <div>
elemento1~elemento2         |p ~ ul                       |Seleciona todos os elementos <ul> que são precedidos por um elemento <p>
[attributo]                 |[target]                     |Seleciona todos os elementos com o atributo target
[atributo=valor]            |[target=_blank]              |Seleciona todos os elementos com o atributo target configurado em _blank / target="_blank"
[atributo~=valor]           |[title~=curso]               |Seleciona todos os elementos cujo o atributo title contenha a palavra "curso"
[atributo|=valor]           |[lang|=pt]                   |Seleciona todos os elementos com um valor de atributo lang começando com "pt"
[atributo^=valor]           |a[href^="https"]             |Seleciona cada elemento <a> cujo valor do atributo href começa com "https"
[atributo$=valor]           |a[href$=".rar"]              |Seleciona cada elemento <a> cujo valor do atributo href termina com ".rar"
[atributo*=valor]           |a[href*="cursos"]            |Seleciona a cada <uma> elemento cujo valor do atributo href contenha a substring "cursos"
:active                     |a:active                     |Seleciona o link ativo
::after                     |p::after                     |Insira algo depois do conteúdo de cada elemento
::before                    |p::before                    |Insira algo antes do conteúdo de cada elemento
:checked                    |input:checked                |Seleciona todos os elementos <input> que tem a propriedade checked
:disabled                   |input:disabled               |Seleciona todos os elementos <input> que tem a propriedade disabled
:empty                      |p:empty                      |Seleciona todos os elementos <p> que não tem filhos (incluindo os nós de texto)
:enabled                    |input:enabled                |Seleciona todos os elementos <input> que tem a propriedade enabled
:first-child                |p:first-child                |Seleciona todos os elementos <p> que são first-child de seu elemento pai
::first-letter              |p::first-letter              |Seleciona a primeira letra de cada elemento <p>
::first-line                |p::first-line                |Selects the first line of every <p> element
:first-of-type              |p:first-of-type              |Seleciona a primeira linha de cada elemento <p>
:focus                      |input:focus                  |Seleciona o elemento de entrada que tem o foco
:hover                      |a:hover                      |Selecione os links que o tem a propriedade hover configurada
:in-range                   |input:in-range               |Seleciona elementos de entrada com um valor dentro de um intervalo especificado
:invalid                    |input:invalid                |Seleciona todos os elementos <input> que tem a propriedade invalid
:lang(language)             |p:lang(en)                   |Seleciona todos os elementos <p> com um atributo lang igual a "en" (inglês)
:last-child                 |p:last-child                 |Seleciona todos os elementos <p> que é o último filho do seu elemento pai
:last-of-type               |p:last-of-type               |Seleciona todos os elementos <p> que é o último elemento <p> de seu elemento pai
:link                       |a:link                       |Seleciona todos os links não clicados
:not(selector)              |:not(p)                      |Seleciona todos os elementos que não são um elemento <p>
:nth-child(n)               |p:nth-child(2)               |Seleciona o elemento <p> que é o segundo filho de seu elemento pai
:nth-last-child(n)          |p:nth-last-child(2)          |Seleciona o elemento <p> que é o segundo filho de seu elemento pai, a contar do último elemento filho
:nth-last-of-type(n)        |p:nth-last-oftype(2)         |Seleciona o elemento <p> que é o segundo elemento <p> de seu elemento pai, a contar do último elemento filho
:nth-of-type(n)             |p:nth-of-type(2)             |Seleciona o elemento <p> que é o segundo elemento <p> de seu elemento pai
:only-of-type               |p:only-of-type               |Seleciona todos os elementos <p> de seu elemento pai
:only-child                 |p:only-child                 |Seleciona todos os elementos <p> que só tem um elemento como filho
:optional                   |input:optional               |Seleciona elementos input com nenhum atributo "required"
:out-of-range               |input:out-of-range           |Seleciona elementos input com um valor fora de um intervalo especificado
:read-only                  |input:read-only              |Seleciona elementos input com o atributo "readonly" especificado
:read-write                 |input:read-write             |Seleciona elementos input com o atributo "readonly" NÃO especificado
:required                   |input:required               |Seleciona elementos input com o atributo "required" especificado
:root                       |:root                        |Seleciona o elemento raiz do documento
::selection                 |::selection                  |Selecciona a parte de um elemento que é selecionado pelo usuário
:target                     |#noticias:target             |Seleciona o elemento #noticias atual (clicou em um URL que contém esse nome de âncora)
:valid                      |input:valid                  |Seleciona todos os elementos input
```

