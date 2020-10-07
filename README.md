# Tag figure

- [X] **`figure`** - Sempre que quisermos acrescentar uma LEGENDA a alguma coisa, usa-se o figure.
  - Display: Block
  - Categoria: Fluxo e Seção
  - Contido por: Fluxo

O elemento figure representa algum conteúdo do fluxo, opcionalmente com uma legenda, que é independente (como uma frase completa) e normalmente é referenciada como uma única unidade a partir do fluxo principal do documento. Assim, o elemento pode ser usado para anotar ilustrações, diagramas, fotos, listagens de código etc. O primeiro filho do elemento figcaption do elemento, se houver, representa a legenda do conteúdo do elemento da figure. Se não houver um elemento filho de legenda, então não haverá legenda. O conteúdo do elemento figure é parte do fluxo circundante. Se o objetivo da página é exibir a figure, por exemplo, uma fotografia em um site de compartilhamento de imagens, os elementos da figure e da figure podem ser usados ​​para fornecer explicitamente uma legenda para essa figure. Para conteúdo que é apenas relacionado tangencialmente ou que serve a um propósito separado do fluxo circundante, o elemento de lado deve ser usado (e pode, por si só, envolver uma figure). Por exemplo, uma citação pull que repete o conteúdo de um artigo seria mais apropriada em um aparte do que em uma figure, porque não faz parte do conteúdo, é uma repetição do conteúdo com o objetivo de atrair leitores ou destacar tópicos principais .

```
<figure>
  
  <figcaption>
    O CONTEÚDO DA QUI E DIRETAMENTE RELACIONADO AO CONTEUDO DENTRO DO <figure> E FORA DO <figcaption>.
  </figcaption>
</figure>
```
