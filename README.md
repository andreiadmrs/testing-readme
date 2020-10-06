# Tag a - Âncora

TAG A - A tag `<a>` server para **links**.

- Display = inline

- `DOM Interface`:
Interface HTMLAnchorElement : HTMLElement {
  attribute DOMString target;
  attribute DOMString download;
  attribute DOMString rel;
  [SameObject, PutForwards=value] readonly attribute DOMTokenList relList;
  attribute DOMString hreflang;
  attribute DOMString type;
  attribute DOMString text;
};
HTMLAnchorElement implements HTMLHyperlinkElementUtils;

## Valores para os atributos

- [X] **`TARGET`** 
  - `_self` - Abre na mesma janela
  - `_blank` - Abre o link em uma nova janela.
  - `_parent` 
  - `_top`
  - `framename`

- [X] **`MEDIA`**
  - `all` - (padrão) Adequado para todos os dispositivos
  - `aural` - Sintetizadores de fala auditiva
  - `braille` - Dispositivod de Braille
  - `handheld` - Dispositivos de tela pequena e banda limitada
  - `projection` - Projetores
  - `print` - Impressoras
  - `screen` - Telas de computador
  - `tv` - Televisores

- [X] **`REL`**
  - `alternate` - Fornece um link para uma representação alternativa do documento (por exemplo, imprimir página, traduzida ou espelhada)
  - `author` - Fornece um link para o autor do documento
  - `bookmark` - URL permanente usado para bookmarking
  - `external` - Indica que o documento referenciado não faz parte do mesmo site que o documento atual
  - `help` - Fornece um link para um documento de ajuda
  - `licence` - Fornece um link para informações de direitos autorais do documento
  - `next` - Fornece um link para o próximo documento da série
  - `nofollow` - Links para um documento não endossado, como um link pago. ("nofollow" é usado pelo Google para especificar que o robô de pesquisa do Google não deve seguir esse link)
  - `noreferrer` - Requer que o navegador não envie um cabeçalho de referência HTTP se o usuário seguir o hyperlink
  - `noopener` - Requer que qualquer contexto de navegação criado seguindo o hiperlink não deva ter um contexto de navegação de abertura
  - `prev` - O documento anterior em uma seleção
  - `search` - links de pesquisa para uma ferramenta de pesquisa para o documento
  - `tag` - Uma tag (keyword) para o documento atual

- [X] **`TYPE`**
- http://www.iana.org/assignments/media-types/media-types.xhtml

```
<a href="link Completo" target="Onde será aberto" rel="Que tpo de arquivo vai ser chamado atraves deste link" media="Indica para qual mídia esse arquivo é mais adequado" hreflang="Idioma da página" type="Que tipo de conteúdo tem na codificação dessa página">Nome Do Link</a>

mailto:Rogerluiz882@gmail.com?cc=Rogerluiz882@gmail.com&bcc=Rogerluiz882@gmail.com&Subject=Assunto%Do%Email&body=Conteudo%do%email"
```
