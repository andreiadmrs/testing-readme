## Padronização de commits

Para poder padronizar seus commits, você vai precisar de duas ferramentas, o [commitlint](https://github.com/conventional-changelog/commitlint) e o [commitizen](https://github.com/commitizen/cz-cli), você pode instalar essas dependências usando o npm ou o yarn.

Caso você não queira ler a documentação, recomendo dois vídeos sobre como usar as ferramentas para padronização:

- Rocketseat - [Padronizando mensagens de commit do Git | Code/Drops #12](https://www.youtube.com/watch?v=erInHkjxkL8).
- Angelo Luz - [Git - Padronização de commits - gitmoji, commitlint e commitizen](https://www.youtube.com/watch?v=49a9M17ZikI&t=975s).

- [X] **Formato da mensagem**: Cada mensagem de commit consiste em um **cabeçalho**, um **corpo** e um **rodapé**. 

- [X] **Cabeçalho**: Tem um formato pré-definido, que inclui um **tipo** e um **título**:

```
<tipo>(<escopo opcional>): <título>

<corpo opcional>

<rodapé opcional>

Exemplos:
fix(integracao-erp): xxxxxxx
improve(app-toolbox): xxxxxxx
docs: Instruções de iniciar projeto com docker
```

- [X] O **cabeçalho** é obrigatório.

Qualquer linha da mensagem do commit não pode ter mais de 100 caracteres! Assim fica mais fácil para ler no GitHub, Gitlab e outras ferramentas de git.

- [X] **Título**: O título contém uma descrição sucinta da mudança:

* use o imperativo, tempo presente: "mudança" não "mudou" nem "muda".
* não capitalize a primeira letra.
* sem ponto (.) no final.

- [X] **Corpo**: Um corpo de mensagem de commit mais longo PODE ser fornecido após o título, fornecendo informações contextuais adicionais sobre as alterações no código. Configure a mensagem com um wrap de 80 caracteres. Use para explicar "o que" e "porque" foi realizado essa modificação, ao invez de "como". O corpo DEVE começar depois de uma linha em branco após a descrição.

- [X] **Rodapé**: Um rodapé PODE ser fornecido depois de uma linha em branco após o corpo. Caso exista um ticket no jira, criar um referência assim: `issue TP-666` ou `closes issue TP-666`.

- [X] **Reverter um commit**: Se o commit reverte um commit anterior, ele deve começar por `revert:`, seguido pelo cabeçalho do commit revertido. No corpo, ele deve dizer: `Isso reverte o commit <hash> .`, onde o hash é o SHA do commit sendo revertido.

## Tipos

Deve ser um dos seguintes:

* **build**: Alterações que afetam o sistema de build ou dependências externas.
* **static**: Alterações no conteúdo de arquivos estáticos (dados .json, imagens, etc).
* **ci**: Alterações em nossos arquivos e scripts de configuração de CI.
* **cd**: Alterações em nossos arquivos e scripts de configuração para CD.
* **docs**: Somente alterações na documentação.
* **feat**: Um novo recurso.
* **fix**: Uma correção de bug da aplicação.
* **perf**: Uma alteração de código que melhora o desempenho.
* **refactor**: Uma alteração de código que não corrige um bug nem adiciona um recurso.
* **improve**: Alguma alteração de código que melhore o comportamento de um recurso.
* **style**: Alterações que não afetam o significado do código (espaço em branco, formatação, ponto e vírgula, etc).
* **test**: Adicionando testes ausentes ou corrigindo testes existentes.
* **revert**: Reverter para um commit anterior.


## Por quê?

* Criação automatizada de CHANGELOGs;
* Determinar automaticamente um aumento de versionamento semântico (com base nos tipos de commits);
* Comunicar a natureza das mudanças para colegas de equipe, o público e outras partes interessadas de forma padronizada
* Disparar processos de build e deploy;
* Facilitar a contribuição de outras pessoas em seus projetos, permitindo que eles explorem um histórico de commits mais estruturado e com melhor rastreabilidade.
