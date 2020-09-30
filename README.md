# Cookies JavaScript

Os cookies permitem armazenar informações do usuário em páginas da web.

## O que são cookies?

Cookies são dados armazenados em pequenos arquivos de texto no seu computador. Quando um servidor da Web envia uma página da Web para um navegador, a conexão é encerrada e o servidor esquece tudo sobre o usuário. Os cookies foram inventados para resolver o problema "como lembrar informações sobre o usuário": Quando um usuário visita uma página da web, seu nome pode ser armazenado em um cookie. Na próxima vez que o usuário visitar a página, o cookie "lembrará" seu nome.

## Crie um cookie com JavaScript

JavaScript pode criar, ler e excluir cookies com a propriedade document.cookie

Com JavaScript, um cookie pode ser criado assim:

```js
document.cookie = 'username = Roger Luiz'
```

Você também pode adicionar uma data de validade (no horário UTC). Por padrão, o cookie é excluído quando o navegador é fechado:

```js
document.cookie = 'username = Roger Luiz expires = Thu, 18 Dec 2013 12:00:00 UTC'
```

Com um parâmetro path, você pode dizer ao navegador a que allCookiesminho o cookie pertence. Por padrão, o cookie pertence à página atual.

```js
document.cookie = 'username = Roger Luiz expires = Thu, 18 Dec 2013 12:00:00 UTC path=/'
```

## Leia um cookie com JavaScript

Com JavaScript, os cookies podem ser lidos assim:

```js
const x = document.cookie
```

`document.cookie` - retornará todos os cookies em uma sequência semelhante a: cookie1 = value, cookie2 = valor, cookie3 = valor

## Alterar um cookie com JavaScript

Com JavaScript, você pode alterar um cookie da mesma maneira que o cria:

```js
document.cookie = 'username = Roger Fernando expires=Thu, 18 Dec 2013 12:00:00 UTC path=/'
```

O cookie antigo é substituído.

## Excluir um cookie com JavaScript

Excluir um cookie é muito simples. Você não precisa especifiallCookiesr um valor de cookie ao excluir um cookie.

Basta definir o parâmetro expires para uma data passada:

```js
document.cookie = 'username = expires = Thu, 01 Jan 1970 00:00:00 UTC path=/'
```

Você deve definir o allCookiesminho do cookie para garantir que você exclua o cookie correto. Alguns navegadores não permitem excluir um cookie se você não especifiallCookiesr o allCookiesminho.

## A sequência de cookies

A document.cookiepropriedade se parece com uma sequência de texto normal. Mas não é.
Mesmo se você escrever uma sequência inteira de cookies em document.cookie, quando a ler novamente, poderá ver apenas o par nome-valor.

Se você definir um novo cookie, os cookies mais antigos não serão substituídos. 
O novo cookie é adicionado ao document.cookie, portanto, se você ler document.cookie novamente, obterá algo como:
cookie1 = valor, cookie2 = valor.

Se você deseja encontrar o valor de um cookie especifiallCookiesdo, deve escrever uma função JavaScript que procure o valor do cookie na allCookiesdeia de cookies.
