# Strings P2 - Métodos

- [X] **`search()`** - O método serach() procura pela ocorrência e retorna sua posição dentro da string, a posição é em relação ao primeiro caractere da ocorrência, veja o código:

```js
const texto = 'Canal Fessor Bruno - Curso de Javascript - CFB'
const resultado = texto.search( /Curso/ )
console.log( resultado )
```

O método "search" irá procurar pela primeira ocorrência da palavra "Curso" com "C" maiúsculo.

**Observação**: Os modificadores que aprendemos anteriormente também podem ser usados no método "search" da mesma
maneira que no método "match".

- [X] **`replace()`** - Este método substitui uma string por outra, simples assim, ele pesquisa a string informada, como no método "match" e a substitui por outra string nas aspas informada como segundo parâmetro, veja o código de exemplo a
seguir que troca o texto "Javascript" pelo texto "React":

```js
const texto = 'Javascript - Node'
const resultado = texto.replace( /Javascript/i , 'React' )
console.log( resultado )
```

Note pelo código que o texto "Javascript - Node" teve a string "Javascript" trocada e foi
impresso o texto "Javascript - React".

- [X] **`charAt()`** - Retorna o caractere na posição indicada como parâmetro do método.

```js
const texto = 'Javascript'
const resultado = texto.charAt( 6 )
console.log( resultado )
```

No código acima o método retorna a letra "r", pois é o caractere que está na posição 6.

- [X] **`charCodeAt()`** - Retorna o código do caractere na posição indicada como parâmetro do método.

```js
const texto = 'Javascript'
const resultado = texto.charCodeAt( 6 )
console.log( resultado )
```

No código acima o método retorna o código a letra "r" que é o código 114, pois é o caractere que está na posição 6.

- [X] **`concat()`** - Concatena, funde, une, junta uma string em outra, no código a seguir juntamos as strings textOne e textTwo.

```js
const textOne = 'React - '
const textTwo = 'Node'
const resultado = textOne.concat( textTwo )
console.log( resultado )
```

- [X] **`fromCharCode()`** - Converte um código informado no caractere correspondente, o script a seguir converte o código 66 no caractere correspondente que é o "B":

```js
const resultado = String.fromCharCode( 66 )
console.log( resultado )
```
