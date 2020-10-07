# Lista de definição, Tags dl, dt e dd

- [X] **`<dl>`** -  O elemento dl representa uma lista de associação que consiste em zero ou mais grupos de nome e valor (uma lista de descrição). Um grupo nome-valor consiste em um ou mais nomes (elementos dt) seguidos por um ou mais valores (elementos dd), ignorando quaisquer nós que não sejam elementos dt e dd. Os grupos nome-valor podem ser termos e definições, tópicos e valores de metadados, perguntas e respostas ou quaisquer outros grupos de dados com valor-nome. dentro de um grupo são alternativas; vários parágrafos que fazem parte do mesmo valor devem ser todos fornecidos no mesmo elemento dd. A ordem da lista de grupos e dos nomes e valores em cada grupo pode ser significativa.
  - Display: Block
  - Categoria: FLuxo
  - Contido por: Fluxo
  - Filhos: `<dt>` e `<dd>` 

- [X] **`<dt>`** - O elemento dt representa o termo, ou nome, parte de um grupo de descrição de termos em uma lista de descrição (elemento dl).
  - Display: Block
  - Categoria: 
  - Contido por: `<dl>` ou `<dialog>`
  - Filhos: Fraseado (textos)

- [X] **`<dd>`** - O elemento dd representa a descrição, definição ou valor, parte de um grupo de descrição de termos em uma lista de descrição (elemento dl).
  - Display: Block
  - Categoria: 
  - Contido por: `<dt>` ou `<dialog>`
  - Filhos: Fluxo
