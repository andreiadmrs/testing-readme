# Strings P1

- [X] **`match()`** - O método match procura um texto especificado em uma string, o método pode retornar o valor procurado como único valor de retorno, um array com todas as ocorrências encontradas ou "null" caso nada seja encontrado.

```js
suaString.match( procura )
```

### Alguns exemplos:

```js
const texto = 'Curso de Javascript'
const resultado = texto.match( 'Javascript' )
console.log( resultado )
```

No código acima criamos uma variável com um texto, em seguida criamos outra variável que vai receber o resultado da busca do método match que está procurando o texto "Javascript". O resultado deste código é a impressão do texto "Javascript" na tela, um detalhe importante é que se for pesquisado o texto "Javascript", com "J" minúsculo o resultado será "null", pois, o padrão é a pesquisa exata.

Quando pesquisamos usando aspas, independentemente do número de ocorrências encontradas a quantidade
informada será sempre 1, ou seja, se tivéssemos 5 palavras "Canal", seria retornado a palavra "Canal" e somente
uma ocorrência.

```js
const texto = 'Canal Canal Canal Canal Canal'
const resultado = texto.match( 'Canal' )
console.log( resultado )
console.log( resultado.length )
```

Como melhorar isto e passar a armazenar os resultados em um array? É simples, basta mudar a forma de passar o
parâmetro e usar um modificador, veja:

```js
const texto = 'Canal Canal Canal Canal Canal'
const resultado = texto.match( /Canal/g )
console.log( resultado[0] )
console.log( resultado.length )
```

Trocamos aspas por barra e usamos o modificador "g", desta maneira as ocorrências são armazenadas uma em cada
posição do vetor.

O modificador "g" diz ao método para encontrar todas as ocorrências da palavra e não parar na primeira
encontrada, podemos ainda usar os modificadores "i" e "m", veja a tabela a seguir:

Modificador   | Descrição
--------------|---------------------------------------------------------------------------------------
i             | Busca sem case-sensitive, ou seja, não diferencia letras maiúsculas de minúsculas
g             | Diz ao método para encontrar todas as ocorrências da palavra e não parar na primeira encontrada, cada ocorrência é armazenada em uma posição do array
m             | Pesquisa normal sem armazenar em forma de array

Agora sabemos como pesquisar ignorando caracteres maiúsculos de minúsculos:

```js
const texto = 'Canal cAnal caNal canAl canaL canal CANAL'
const resultado = texto.match(/canal/gi)
console.log(resultado[0] + '<br>')
console.log(resultado.length)
```

Note que agora usamos dois modificadores "g" e "i".

Vamos a mais uma pequena alteração em nosso código tirando o índice do array:

```js
const texto = 'Canal cAnal caNal canAl canaL canal CANAL'
const resultado = texto.match( /canal/gi )
console.log( resultado )
console.log( resultado.length )
```

Agora são impressos todas as ocorrências de uma só vez

Quer procurar por letras? O processo é o mesmo, veja a alteração do código onde procuramos por ocorrências da
letra "o" e imprimimos a quantidade de letras "o" encontradas:

```js
const texto = 'Curso de Javascript'
const resultado = texto.match( /o/gi )
console.log( resultado.length )
```

Ainda podemos melhorar nossa pesquisa usando colchetes, por exemplo, se for preciso pesquisar todas as letras "a"
e "o"? É simples:

```js
const texto = 'Curso de Javascript'
const resultado = texto.match( /[oa]/gi )
console.log( resultado.length )
```

O resultado sete é relativo ao número de letras "a" somado ao número de letras "o".

Confira a seguir uma tabela com outras opções de pesquisa usando colchetes:

Expressão   | Descrição
------------|---------------------------------------------------------------------------------------
[abcd]      | Pesquisa pelos caracteres "a", "b", "c" e "d"
[^ab]       | Pesquisa por todos os caracteres, menos os "a" e "b".
[a-f]       | Pesquisa pelos caracteres de "a" até "f"
[^a-f]      | Pesquisa por todos os caracteres, menos os de "a" até "f"
[a|f]       | Pesquisa pelos caracteres "a" e "f", semelhante à primeira opção.

Outras opções que podemos para implementar nossa pesquisa são os "metacaracteres", por exemplo, se
precisarmos saber quantos espaços existem na string, basta usar o "metacaractere" espaço, veja o exemplo a seguir:

```js
const texto = 'Curso de Javascript'
const resultado = texto.match( /\s/g )
console.log( resultado.length )
```

Assim obtemos a contagem dos espaços.

Existem vários "metacaracteres" que podemos usar, confira a tabela a seguir:

Metacaratere   | Descrição
---------------|-----------------------------------------------------------------------------------
\w             | Pesquisa somente por letras e numerais, ignorando espaços, traços, etc.
\W             | Pesquisa por caracteres diferentes de números e letras
\d             | Pesquisa por numerais
\D             | Pesquisa por todos os caracteres que não são numerais
\s             | Pesquisa pelos espaços
\S             | Pesquisa por todos os caracteres, menos os espaços
\b             | Pesquisa por ocorrência que iniciem ou terminem com uma letra ou número, cada ocorrência que iniciar e terminar com um número ou letra conta como 2
\B             | Pesquisa por ocorrência que NÃO iniciem ou terminem com uma letra ou número
\O             | Procura por caracteres nulos.
\n             | Procura por quebra de linha.
\r             | Procura por caractere de "retorno de carro" ENTER.
\t             | Procura por caractere de tabulação TAB
\v             | Procura por caractere de tabulação vertical
s+             | Procura por palavras que contenham uma ou mais letras "s"
