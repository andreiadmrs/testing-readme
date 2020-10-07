# Formulário P1

- [X] **`<form>`** - O elemento do form representa uma coleção de elementos associados ao formulário, alguns dos quais podem representar valores editáveis ​​que podem ser enviados a um servidor para processamento. O atributo accept-charset fornece as codificações de caracteres que devem ser usadas para o envio. Se especificado, o valor deve ser um conjunto ordenado de tokens separados por espaço exclusivos que não fazem distinção entre maiúsculas e minúsculas ASCII e cada token deve ser uma correspondência que não diferencia maiúsculas de minúsculas de ASCII para um dos rótulos de uma codificação de caracteres compatível com ASCII. [ENCODING] O atributo name representa o nome do formulário na coleção de formulários. O valor não deve ser a cadeia vazia e o valor deve ser exclusivo entre os elementos do formulário na coleção de formulários em que ele está, se houver. O atributo de preenchimento automático é um atributo enumerado. O atributo tem dois estados. A palavra-chave on mapeia para o estado ligado e a palavra-chave off mapeia para o estado desligado. O atributo também pode ser omitido. O valor padrão ausente é o estado ligado. O estado desativado indica que, por padrão, os controles do formulário terão o nome do campo de preenchimento automático definido como "desativado"; o estado on indica que, por padrão, os controles do formulário terão o nome do campo de preenchimento automático definido como "on". Os atributos action, enctype, method, novalidate e target são atributos para envio do formulário.
  - Display: Block
  - Categoria: FLuxo
  - Contido por: Fluxo
  - Filhos: FLuxo

**Atributos (form):** action, method, enctype, name, accept-charset, novalidate, target, autocomplete.

**Elementos do form:** button, fieldset, input, keygen, label, object, output, select, textarea, option, optgroup

## Atributos para o form

- `action`: URL com o arquivo que irá receber os dados enviados.
- `method`: Método d envio dos daos (get ou post).
- `enctype`: Codificação (tipo) dos dados enviados.
- `name`: Nome do formulário.
- `accept-charset`: especifica as codificações de caracteres que devem ser usadas para o envio do formulário.
- `novalidate`: Desabilita a validação pelo browser.
- `target`: Como a página de destino (action) será aberta.
- `autocomplete`: Autocompletar campos ativo.

- [X] **`<label>`** - A tag label define um rótulo para um elemento. (Vem antes do input)

```
<label for"">Texto</label>
```

O atributo **for** especifica a qual elemento do formulário um rótulo está vinculado.
O atributo for faz um tipo de link entre a label e o input. Logo o for tem que apontar para o **ID** do **input**.

- [X] **`<input>`** - A tag input especifica um campo de entrada onde o usuário pode inserir dados.

```
<input type="tipo" name="nome">
```

## Valore pata o type

- `button`: Um botão sem comportamento padrão.
- `checkbox`: Uma caixa de marcação. Você deve usar o atributo value para definir o valor enviado por este item. Use o atributo checked para indicar se o item está selecionado por padrão. Você também pode usar o atributo indeterminate para indicar que a caixa de marcação está em um estado indeterminado (na maioria das plataformas, isso desenha uma linha horizontal cortando a caixa).
- `color`: HTML5 Um controle para especificar cores. A interface de um seletor de cores não tem nenhuma funcionalidade obrigatória a não ser aceitar cores simples em texto (mais informações — em inglês).
- `date`: HTML5 Um controle para inserir uma data (ano, mês e dia, sem horário).
- `datetime`: HTML5 Um controle para inserir data e horário (hora, minuto, segundo e fração de segundo) baseado no fuso horário UTC.
- `datetime-local`: HTML5 Um controle para inserir data e horário, sem fuso horário.
- `email`: HTML5 Um campo para editar um endereço de e-mail. O valor do campo é validado para estar vazio ou ter um único endereço de e-mail válido antes de ser enviado. As pseudoclasses CSS :valid e :invalid são aplicadas apropriadamente.
- `file`: Um controle que permite ao usuário selecionar um arquivo. Use o atributo accept para definir os tipos de arquivo que o controle pode selecionar.
- `hidden`: Um controle que não é exibido mas cujo valor é enviado ao servidor.
- `image`: Um botão gráfico para enviar o formulário. Você deve usar o atributo src para definir a fonte da imagem e o atributo alt para definir um texto alternativo. Você pode usar os atributos height e width para definir o tamanho da imagem em pixels.
- `month`: HTML5 Um controle para inserir mês e ano, sem fuso horário.
- `number`: HTML5 Um controle para inserir um número de ponto flutuante.
- `password`: Um campo de texto com uma só linha cujo valor é obscurecido. Use o atributo maxlength para especificar o comprimento máximo do valor que pode ser inserido.
- `radio`: Um botão de escolha. Você deve usar o atributo value para definir o valor a ser enviado por este item. Use o atributo checked para indicar se este item deve estar selecionado por padrão. Botões de escolha que têm o mesmo valor para o atributo name estão no mesmo "grupo de botões de escolha"; apenas um botão de escolha no grupo pode estar selecionado de cada vez..
- `range`: HTML5 Um controle para inserir um número cujo valor exato não é importante. Este tipo de controle usa os seguintes valores padrão se os atributos correspondentes não forem especificados:
  - min: 0
  - max: 100
  - value: min + (max-min)/2, ou min se max for menos que min
  - step: 1
- `reset`: Um botão que faz o conteúdo do formulário voltar a ter seus valores padrão.
- `search`: HTML5 Um campo de texto com uma só linha para digitar termos de busca; quebras de linha são automaticamente removidas do valor entrado.
- `submit`: Um botão que envia o formulário.
- `tel`: HTML5 Um controle para inserir um número de telefone; quebras de linha são automaticamente removidas do valor entrado, mas nenhuma outra sintaxe é imposta. Você pode usar atributos como pattern e maxlength para restringir os valores inseridos no controle. As pseudoclasses CSS :valid e :invalid são aplicadas apropriadamente.
- `text`: Um campo de texto com uma só linha; quebras de linha são automaticamente removidas do valor entrado.
- `time`: HTML5 Um controle para inserir um horário sem fuso horário.
- `url`: HTML5 Um campo para editar uma URL. O valor inserido é validado para ser vazio ou uma URL absoluta válida antes de ser enviado. Quebras de linha e espaços em branco antes e após o valor inserido são automaticamente removidos. Você pode usar atributos como pattern e maxlength para restringir os valores inseridos no controle. As pseudoclasses CSS :valid e :invalid são aplicadas apropriadamente.
- `week`: HTML5 Um controle para inserir uma data consistindo de ano da semana e número da semana sem fuso horário.
