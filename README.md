# Tag embed

- [X] **`<embed>`** - A tag embed vai representar uma área com um ponte de interação com um arquivo externo geralemnte esse arquivo NÃO HTML.
  - Categoria: Fluxo, Fraseado, Incorporado
  - Contido por: Onde incorporado é esperado
  - Filhos: None

O elemento embed fornece um ponto de integração para um aplicativo externo (normalmente não HTML) ou conteúdo interativo. O atributo src fornece o endereço do recurso que está sendo incorporado. O atributo, se presente, deve conter um URL não vazio válido potencialmente cercado por espaços. O atributo type, se presente, fornece o tipo MIME pelo qual o plug-in a instanciar é selecionado. O valor deve ser um tipo MIME válido. Se o atributo type e o src estiverem presentes, o atributo type deverá especificar o mesmo tipo que os metadados explícitos Content-Type do recurso fornecido pelo src attribute. Qualquer atributo namespace-less que não seja name, align, hspace, e vspace podem ser especificados no elemento embed, desde que o nome seja compatível com XML e não contenha letras ASCII maiúsculas. Esses atributos são passados como parâmetros para o plug-in. O elemento embed suporta atributos de dimensão.
