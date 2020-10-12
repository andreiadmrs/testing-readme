# Formulário P4 (date, time, datetime-local)

Datas e Horas - Campo pré configurado para entrada de valores como datas e horas, possui algumas variações 
descritas a seguir.

- [X] **`datetime-l
```
<form>
  <label>Hora</label>
  <input type="time" name="hora">
</form>
```

- [X] **`datetime`** – Campo para entrada de datas e horas gerais, não possui pré formatação

```
<form>
  <label>Datas e Horas</label>
  <input type="datetime" name="datahora">
</form>
```

## Propriedades para os campos datetime

Propiedade     | Descrição                                                                    | Exemplo
---------------|------------------------------------------------------------------------------|---------------------------------------
name           | Nome do campo                                                                | name=“dataHora”
disabled       | Desabilita o campo não podendo ser editado                                   | disabled=“disabled” ou disabled
form           | Permite especificar a qual formulário o elemento pertence através do ID      | form=“id do formulário pai”
autocomplete   | Permite que o campo seja auto completado ou não                              | autocomplete=“on” ou “off”
autofocos      | Posicione o cursor no elemento automaticamente ao abrir a página             | autofocos=“autofocus” ou autofocus
maxlength      | Número máximo de elementos que podem ser inseridos no campo                  | maxlength=“50”
pattern        | Especifica uma expressão para validação do campo                             | pattern=“\d{5}”
readonly       | Especifica que o campo é “somente leitura”, não permite editar o conteúdo    | readonly=“readonly” ou readonly
required       | Especifica que o campo é requerido, tornando-o obrigatório                   | required=“required” ou required
size           | Tamanho visível do elemento                                                  | size=“30”
placeholder    | Texto (hint) de exemplo não editável é apagado ao inserir o valor no campo   | placeholder=“Digite seu nome aqui”
value          | Valor inicial do campo                                                       | value=“jogador1”
list           | Especifica uma lista pelo ID que contém os valores para o campo              | list=“id da lista”
min            | Valor mínimo do campo                                                        | min=“valor mínimo”
max            | Valor máximo permitido no campo                                              | max=“valor máximo”
step           | Passo de incremento ou decremento do campo                                   | step=“valor do passo”
