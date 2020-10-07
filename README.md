# Formulário P2

- [X] **`tel`** - O campo “tel” serve para entrada de número de telefone, porém, como não existe um padrão mundial, não existe
máscara nem validação nativas.

```
<form>
  <label>Telephone:<label/>
  <input type="tel" name="telefone">
</form>
```

## Propriedades para tel

Propiedade      | Descrição                                                                   | Exemplo
----------------|-----------------------------------------------------------------------------|---------------------------------------
name            | Nome do campo                                                               | name=“telefone”
disabled        | Desabilita o campo não podendo ser editado                                  | disabled=“disabled” ou disabled
form            | Permite especificar a qual formulário o elemento pertence através do ID     | form=“id do formulário pai”
autocomplete    | Permite que o campo seja auto completado ou não                             | autocomplete=“on” ou “off”
autofocos       | Posicione o cursor no elemento automaticamente ao abrir a página            | autofocos=“autofocus” ou autofocus
maxlength       | Número máximo de elementos que podem ser inseridos no campo                 | maxlength=“50”
pattern         | Especifica uma expressão para validação do campo                            | pattern=“\d{5}”
readonly        | Especifica que o campo é “somente leitura”, não permite editar o conteúdo   | readonly=“readonly” ou readonly
required        | Especifica que o campo é requerido, tornando-o obrigatório                  | required=“required” ou required
size            | Tamanho visível do elemento                                                 | size=“30”
placeholder     | Texto (hint) de exemplo não editável é apagado ao inserir o valor no campo  | placeholder=“Digite seu nome aqui”
value           | Valor inicial do campo                                                      | value=“jogador1”
list            | Especifica uma lista pelo ID que contém os valores para o campo             | list=“id da lista”
