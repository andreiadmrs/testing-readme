# Strings P4 - Método

- [X] **`toString()`** - Converte um valor qualquer em uma string.

```js
const number = 10
const resultado = number.toString()
console.log( resultado )
```

Será impresso o numeral 10.

Uma forma de uso muito interessante do método toString é a possibilidade de retornar o numeral indicado na base,
2, base 8 ou base 16, ou seja, converter em binário, octal ou hexadecimal, veja o código de exemplo.

```js
const decimal = 15
const binario = decimal.toString( 2 )
const octal = decimal.toString( 8 )
const hexadecimal = decimal.toString( 16 )
console.log( decimal )
console.log( binario )
console.log( octal )
console.log( hexadecimal )
```

O código acima converte o numeral 15 para as bases, 2, 8 e 16, veja o resultado.

- [X] **`trim()`** - Remove os espaços antes e depois da string especificada. No código abaixo serão removidos todos os espaços no início e no final da string, os espaços no meio da string não são removidos.

```js
const string = ' Aprendendo Javascript '
const resultado = string.trim()
console.log( resultado )
```

- [X] **`substring()`** - O método substring() extrai os caracteres de uma string, entre dois índices especificados, e retorna a nova sub string. Este método extrai os caracteres em uma sequência entre "start" e "end", sem incluir o próprio "end". Se "start" for maior que "end", esse método trocará os dois argumentos, significando str.substring(1, 4) == str.substring(4, 1). Se "start" ou "end" for menor que 0, será tratado como se fosse 0. O método substring() não altera a sequência original.

```js
const string = 'Hello World!'
const resultado = string.substring( 6 )
console.log( resultado )
```

## Usando caracteres especiais na string

Em alguns momentos vamos precisar usar aspas, adicionar tabulação, quebra de linha, etc, em nossas strings e para
estes casos temos que indicar estes caracteres dentro da string, veja um exemplo a seguir de uma string com aspas.

```js
const string = 'Aprendendo Javascript - \'JS\' - Curso de Javascript'
console.log( string )
```

Código  | Descrição
--------|----------------------------
\n      | Quebra de linha.
\r      | Retorno de carro, ENTER
\t      | Tabulação TAB
\b      | Backspace
\f      | Form feed, adiciona um espaço
