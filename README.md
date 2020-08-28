# Background PT 1

Propiedade                     | Descrição
------------------------------ |----------------------------------------------------------------------
background-color: cor;         | Especifica a cor de fundo de um elemento.
background-image: url(imagem); | Especifica uma imagem a ser usada como plano de fundo de um elemento.
background-size: VALOR VALOR;  | largura e altura, permite controlar a dimensão da imagem.

- [X] background-repeat - Controla a repetição de uma imagem:

Propiedade                    | Descrição
----------------------------- |----------------------------------------
background-repeat: repeat;    | Repete a imagem (padrão)
background-repeat: no-repeat; | Não repete a imagem
background-repeat: repeat-x;  | Repete a imagem apenas na horizontal
background-repeat: repeat-y;  | Repete a imagem apenas na vertical<br>

- [X] background-position - Controla a posição da imagem:

Propiedade                          | Valor
------------------------------------|----------------------
background-position: EIXOX EIXOY;   | Variante
background-position: left top;      | Esquerda em cima
background-position: left center;   | Esquerda no centro
background-position: left bottom;   | Esquerda em baixo
background-position: right top;     | Direita em cima
background-position: right center;  | Direita no centro
background-position: right bottom;  | Direita em baixo
background-position: center top;    | Centro no topo
background-position: center center; | Centro no centro
background-position: center bottom; | Centro em baixo


Podemos colocar mais de uma imagem no background:
```
Seletor {
  background-color: #XXX;
  background-image: url(Imagem1), url(Imagem2);
  background-size: Imagem1px, Imagem2px;
  background-repeat: Imagem1, Imagem2;
  background-position: Imagem1, Imagem2;
}
```
