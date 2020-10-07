# Tag dfn

- [X] **`dfn`** - A tag dfn basicamente é uma tag que marca o termo de uma determinada definição
  - Display: Inline
  - Categoria: Fluxo e Fraseado
  - Contido por: Fraseado
  - Filhos: Fraseado

O elemento dfn representa a instância que define um termo. O parágrafo, o grupo da lista de descrição ou a seção que é o ancestral mais próximo do elemento dfn também deve conter as definições para o termo fornecido pelo elemento dfn.Definição do termo: Se o elemento dfn tiver um atributo title, o valor exato O valor desse atributo é o termo que está sendo definido. Caso contrário, se contiver exatamente um nó filho do elemento e nenhum nó filho do Texto, e esse elemento filho for um elemento abbr com um atributo title, o valor exato desse atributo será o termo que está sendo definido. Caso contrário, é o textContent exato do elemento dfn que fornece o termo sendo definido.Se o atributo title do elemento dfn estiver presente, ele deverá conter apenas o termo sendo definido.Um elemento que vincula a um elemento dfn representa um instância do termo definido pelo elemento dfn.

## Atributos

- `title`: texto que será mostrado quando o mouse for parado em cima da palavra

## Diferençã entre abbr e dnf:

O elemento dfn marca um termo a ser definido no próprio documento ou em um documento externo. Geralmente é utilizado como item de um glossário ou em uma explicação didática.

O elemento abbr, junto com o atributo title, permite indicar o significado de uma determinada sigla ou abreviação que foi definida pelo elemento dfn.

## Exemplo

```
<p> A expressão <dfn>Ouvido Absoluto</dfn> indica a capacidade que um músico tem de identificar a altura de uma nota musical sem nenhuma referência prévia</p>

<p>Na linguagem musical, o termo <dfn><abbr title="Da capo">D.C</abbr></dfn> significa que um determinado trecho musical deve ser repetido desde o seu começo e tem origem na expressão italiana <span lang="it"><i>da capo</i></span> que significa da cabeça ou do início.</p>
```
