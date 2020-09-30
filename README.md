# ScrollIntoView

Este método rola a página até que o elemento indicado como parâmetro esteja no topo da janela.
O método Element.scrollIntoView() move o elemento ao qual é aplicado para a área visível da janela do navegador.

- `element.scrollIntoView()`                      // Equivalente a element.scrollIntoView(true)
- `element.scrollIntoView( alignToTop )`            // Argumentos booleanos
- `element.scrollIntoView( scrollIntoViewOptions )` // argumento Objeto

- `alignToTop` (opcional) - o parâemtro alignToTop é um valor Boolean. Se true, a parte superior do elemento ficará alinhada com o topo da área visível do elemento-pai. Correponde a scrollIntoViewOptions: **`{block: "start", inline: "nearest"}`**. Este é o valor default.

Se false, a parte inferior do elemento ficará alinhada com o fundo da área visível do elemento-pai. 
Corresponde a scrollIntoViewOptions: **`{block: "end", inline: "nearest"}`**

- `scrollIntoViewOptions` (opcional): o parâemtro `scrollIntoViewOptions` é um booleano ou um objeto com as seguintes opções:

```js
{
  behavior: "auto"  | "instant" | "smooth",
  block:    "start" | "center" | "end" | "nearest",
  inline:   "start" | "center" | "end" | "nearest"
}
```

Caso seja um valor booleano, true corresponde a **`{block: "start"}`** e false a **`{block: "end"}`**.
