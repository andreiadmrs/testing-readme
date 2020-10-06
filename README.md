# Tag br, quebra de linha

- [X] **`Tag br: (Break Line)`**
  - Display: Inline
  - Categoria: Fluxo e FrasEado
  - Contido por: Fraseado
  - Filhos: None

O elemento br representa uma quebra de linha. Os elementos br devem ser usados apenas para quebras de linha que realmente fazem parte do conteúdo, como em poemas ou endereços. Os elementos br não devem ser usados para separar grupos temáticos em um parágrafo. Se um parágrafo consistir em nada além de um único elemento br, ele representa uma linha em branco do espaço reservado (por exemplo, como em um modelo). Essas linhas em branco não devem ser usadas para fins de apresentação.


O exemplo a seguir é o uso correto do elemento br:

```
<p>P. Sherman<br>
42 Wallaby Way<br>
Sydney</p>
```

Os exemplos a seguir não são conformes, pois abusam do elemento br:

```
<p><a ...>34 comments.</a><br>
<a ...>Add a comment.</a></p>

<p><label>Name: <input name="name"></label><br>
<label>Address: <input name="address"></label></p>
```

Aqui estão alternativas para os exemplos acima, que estão corretas:

```
<p><a ...>34 comments.</a></p>
<p><a ...>Add a comment.</a></p>

<p><label>Name: <input name="name"></label></p>
<p><label>Address: <input name="address"></label></p>
```
