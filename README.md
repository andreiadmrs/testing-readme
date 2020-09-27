# Strings P3 - Método

- [X] **`indexOf()`** - Retorna a posição do primeiro caractere especificado a ser encontrado, no exemplo procuramos a posição da letra "d" e será retornada a posição 5:

```js
const string = 'Aprendendo Javascript'
const resultado = string.indexOf( 'd' )
console.log( resultado )
```

- [X] **`lastIndexOf()`** - Retorna a posição do último caractere especificado a ser encontrado, no exemplo procuramos a posição da última letra "a" e será retornada a posição 14:

```js
const string = 'Aprendendo Javascript'
const resultado = string.lastIndexOf( 'a' )
console.log( resultado )
```

O resultado deste script é o valor 14 que é a posição da última letra "a" já que a primeira está na posição "12".

- [X] **`localeCompare()`** - Este método compara duas strings, se forem iguais retorna "0" zero, se a primeira for menor que a segunda retorna "-1" e se for maior, retorna "1", então qualquer valor diferente de zero significa que as strings não são iguais. Em nosso código de exemplo o valor impresso será "0" zero, pois, as strings são idênticas.

```js
const string1 = 'Javascript'
const string2 = 'Javascript'
const resultado = string1.localeCompare( string2 )
console.log( resultado )
```

- [X] **`slice()`** - O método slice() corta uma string de um ponto A até um ponto B especificados e retorna o valor recortado, nosso script a seguir retorna o texto "Javascript":

```js
const string = 'Aprendendo Javascript'
const resultado = string.slice( 11 , 21 )
console.log( resultado )
```

Observe que foi recortado da posição 11 até a 21 e retornado o texto "Javascript".

Podemos usar o método slice() com somente um parâmetro, desta maneira como no exemplo a seguir:

```js
const string = 'Aprendendo Javascript'
const resultado = string.slice( 11 )
console.log( resultado )
```

Desta maneira todo conteúdo antes da posição 11 será eliminado e será retornado o texto "Javascript".

Podemos usar o método slice() em vetores também:

```js
const transportes = [ 'avião' , 'moto' , 'carro' , 'trem' , 'navio' ]
const terrestres = transportes.slice( 1 , 4 )
console.log( terrestres )
```

Serão armazenado no array terrestres os transportes moto, carro e trem.

- [X] **`split()`** - O método split() subdivide uma string sempre que encontrar o caractere especificado como divisor, no nosso código definimos o caractere divisor sendo o espaço, desta maneira será criado um array e em cada posição do array será inserida uma ocorrência.

```js
const string = 'Aprendendo Javascript'
const resultado = string.split( ' ' )
console.log( resultado.length )
```

O resultado deste script é dois, pois temos uma string com duas palavras separadas com espaços uma da outra, então a palavra "Aprendendo" fica na posição [0], "Javascript" fica na posição [1].

Caso seja necessário criar um array com as letras separadas basta usar como o exemplo a seguir.

```js
const string = 'Aprendendo Javascript'
const resultado = string.split( '' )
console.log( resultado.length )
```

Neste código o valor retornado como tamanho do array é 21, pois, agora cada caractere será armazenado em
uma posição do array.

Ainda podemos indicar um limite para a divisão, veja o código a seguir que especifica um limite de 2, ou seja será feito o split, porém somente até a segunda ocorrência, então o código a seguir retorna "Aprendendo,Javascript".

```js
const string = 'Aprendendo Javascript'
const resultado = string.split( ' ' , 2 )
console.log( resultado )
```

- [X] **`substr()`** - O método substr() funciona de forma semelhante ao método slice(), com uma diferença básica no segundo parâmetro, que indica o tamanho do corte, veja o exemplo que retorna o texto "Java", indicamos o início do corte na posição 11 e o tamanho como 4, então, a partir da posição 11 serão recortados os 4 caracteres.

```js
const string = 'Aprendendo Javascript'
const resultado = string.substr( 11 , 4 )
console.log( resultado )
```

- [X] **`toLowerCase()`** - Converte a string inteira para caracteres minúsculos, veja o código de exemplo.

```js
const string = 'Aprendendo Javascript'
const resultado = string.toLowerCase()
console.log( resultado )
```

O resultado do código será o texto todo com letras minúsculas.

- [X] **`toUpperCase()`** - Converte a string inteira para caracteres maiúsculos, veja o código de exemplo.

```js
const string = 'Aprendendo Javascript'
const resultado = string.toUpperCase()
console.log( resultado )
```

O resultado do código será o texto todo com letras maiúsculas.
