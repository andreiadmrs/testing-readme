# Tags blockquote e cite, trabalhando com citações

- [X] **`<blockquote>`** - A tag blockquote vai representar uma citação longa.
  - Display: Block
  - Categoria: Fluxo e Seção
  - Contido por: Fluxo
  - Filho: Fluxo

**Dica:** use `<q>` para cotações em linha (curtas).

- [X] **`<cite> (Atributo)`** - URL Especifica a fonte da cotação

DOM Interface:
Interface HTMLQuoteElement : HTMLElement {
attribute DOMString cite;
};


- [X] **`<cite> (Tag)`** - A tag cite vai representar um título de uma obra, ou uma referência aos autores A tag `<cite>` define o título de uma obra (por exemplo, um livro, uma música, um filme, um programa de TV, uma pintura, uma escultura etc.). Nota: O nome de uma pessoa não é o título de uma obra.
  - Display: Inline
  - Categoria: Fluxo e Fraseado
  - Contido por: Fraseado
  - Filho: Fraseado

DOM Interface:
Uses HTMLElement;
