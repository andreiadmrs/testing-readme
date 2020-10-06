# Tags area e map

A tag area trabalha em conjunto com a tag map.
A tag area vai definir uma área clicável, TODOS os parâmetros da tag `<a>` podem ser usados na tag `<area>`

```
<img src="NomeDaImagem" usemap="NomeDoMap">
<map name="NomeDoMap">
  <area shape="Forma geométrica do map" coords="Cordenadas da area clicavel" href="Link" alt="Texto alternatico Caso a imagem não carregue">
</map>
```

- **`shape`**
  - rect = Retângular = APENAS a cordenanda inicial e a final
  - circle = Circular = informa a cordenada do centro + Cordenada do raio
  - poly = Polígono = Quanto mais cordenadas melhor

- [X] **`<area>`**
  - Display: None (Nenhum)
  - Categoria: Fluxo e Fraseado
  - Contido por: <map>
  - Filhos: None (vazio)

Interface HTMLAreaElement: HTMLElement{

  attribute DOMString alt;

  attribute DOMString coords;

  attribute DOMString shape;

  attribute DOMString target;

  attribute DOMString download;

  attribute DOMString rel;

  [SameObject, PutForwards=value] readonly attribute DOMTokenList relList;

  attribute DOMString hreflang;

  attribute DOMString type;

  attribute DOMString referrerPollcy;

};

HTMLAreaElement implements

HTMLHyperlinkElementUtlls;
