## Git

### Instalação

https://git-scm.com/download

### Documentação

https://git-scm.com/doc

## CENAS

- [x] Você deseja criar pontos na história da produção do seu projeto
- [x] Você deseja verificar mudanças feitas no seu projeto

- [x] Você começa uma nova funcionalidade no seu projeto, sem estragar o que já foi feito.
- [x] Você adiciona as novas funcionalidades ao seu projeto em produção
- [x] Você quer deletar a branch da nova funcionalidade, depois de aplicar em seu projeto.

- [x] Você quer colocar seu projeto na nuvem.

- [x] Você vai pegar um projeto já iniciado, para trabalhar com o time
- [x] Você precisa resolver um conflito.
- [x] Antes de enviar a resolução, precisamos atualizar o projeto local.

- [x] Você precisa voltar um arquivo para um determinado momento da linha do tempo.
- [x] Você precisa recuperar algo deletado.

## COMANDOS

- **`git init`** - Cria um repositório Git vazio ou reinicialize um existente.

- **`git status`** - Informa o estado das alterações do nosso projeto.

- **`git add [file]`** - Adiciona ou atualiza mudanças para irem para o repositório.
- **`git add .`** - Você pode adicionar todos os arquivo usando o " . ".

- **`git commit -m "message"`** - Registra alterações no repositório.
- **`git commit -am "message"`** - Atualiza o repositório e registra alterações no repositório ao mesmo tempo.

- **`git log`** - Mostra os pontos na "linha do tempo" do repositório ( commit ).
- **`git log --oneline`** - Mostra os pontos na "linha do tempo" de forma mais resumida.
- **`git log --abbrev-commit`** - Ao vez de mostrar o hash com 40 caracteres, mostra apenas com 7 caracteres.
- **`git log --pretty=oneline`** - Faz com que caiba tudo em uma linha.
- **`git log --graph`** - Desenha uma representação gráfica dos commits no lado esquerdo da saída.

- **`git diff`** - Mostra o que foi alterado em um arquivo, de vermelho o que foi excluído de verde o que foi adicionando.
Use o "git diff" antes de dar o "git add".

- **`git show`** - Apresenta o último ponto na "história" do nosso projeto.
- **`git show [hash]`** - Apresenta determinado ponto na "história" do nosso projeto.

- **`git branch`** - Lista, cria ou exclui ramificações.

- **`git checkout [hash]`** - Alterna ramificações ou restaura arquivos da árvore de trabalho.
- **`git checkout [arquivo_modificado]`** - Descarta as mudanças feitas no arquivo. Use antes de dar o "git add".
- **`git checkout -b [minha-feature]`** - Cria uma nova ramificação no nosso projeto.
- **`git checkout master`** - Vai para a ramificação master.
- **`git checkout [minha_ramificação]`** - Vai para a ramificação criada pelo desenvolvedor.

- **`git reset HEAD`** - Remove um arquivo adicionado pelo "git add". Usar depois do "git add" e antes do "git commit".
- **`git reset --hard [hash]`** - Remove um commit.

- **`git merge [minha_ramificação]`** - Faz a fusão de uma ramificação x com a ramificação master. Para fazer a fusão você tem que estar na ramificação master.

- **`git remote`** - Verifica se existe um repositório remoto.

- **`git push`** - Envia alterações locais para o repositório remoto.

- **`git clone [link_repositório]`** - Clonar um projeto / repositório. 

- **`git pull`** - Puxa do repositório remoto.

Exemplo de um hash:
  - a96c4c3
  - a96c4c3936dbaa78be7254eb7b6b9b86fc46adc0

O que é uma ramificação?

> As ramificações do Git são um indicador efetivo de um instantâneo de suas mudanças. Quando você quiser adicionar um novo recurso ou corrigir um bug—não importa o tamanho, grande ou pequeno—basta criar uma nova ramificação para encapsular as mudanças. Isso faz com que seja mais difícil um código instável ser mesclado com a base de código principal e dá a chance de você limpar seu histórico futuro antes de fazer a mesclagem na ramificação principal.  

## Padronização de commits

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

## Tipo

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

- [X] **Título**: O título contém uma descrição sucinta da mudança:

* use o imperativo, tempo presente: "mudança" não "mudou" nem "muda".
* não capitalize a primeira letra.
* sem ponto (.) no final.

- [X] **Corpo**: Um corpo de mensagem de commit mais longo PODE ser fornecido após o título, fornecendo informações contextuais adicionais sobre as alterações no código. Configure a mensagem com um wrap de 80 caracteres. Use para explicar "o que" e "porque" foi realizado essa modificação, ao invez de "como". O corpo DEVE começar depois de uma linha em branco após a descrição.

- [X] **Rodapé**: Um rodapé PODE ser fornecido depois de uma linha em branco após o corpo. Caso exista um ticket no jira, criar um referência assim: `issue TP-666` ou `closes issue TP-666`.

- [X] **Reverter um commit**: Se o commit reverte um commit anterior, ele deve começar por `revert:`, seguido pelo cabeçalho do commit revertido. No corpo, ele deve dizer: `Isso reverte o commit <hash> .`, onde o hash é o SHA do commit sendo revertido.

## Por quê?

* Criação automatizada de CHANGELOGs;
* Determinar automaticamente um aumento de versionamento semântico (com base nos tipos de commits);
* Comunicar a natureza das mudanças para colegas de equipe, o público e outras partes interessadas de forma padronizada
* Disparar processos de build e deploy;
* Facilitar a contribuição de outras pessoas em seus projetos, permitindo que eles explorem um histórico de commits mais estruturado e com melhor rastreabilidade.

## ALIAS
Você pode criar alias para os comandos do git, basta ir no arquivo ".gitconfig" e definir seus alias.
No uninx ( Linux e Mac ) o arquivo ".gitconfig" fica localizado em: /home/seuusuário/.gitconfig

Alias que eu gosto de usar:

```
[alias]
  i = init
  a = add
  ci = commit
  co = checkout
  cm = checkout master
  cb = checkout -b
  st = status -sb
  sf = show --name-only
  pom = push origin master -u
  ps = push
  lg = log --pretty=format:'%Cred%h%Creset %C(bold)%cr%Creset %Cgreen<%an>%Creset %s' --max-count=30
  incoming = !(git fetch --quiet && git log --pretty=format:'%C(yellow)%h %C(white)- %C(red)%an %C(white)- %C(cyan)%d%Creset %s %C(white)- %ar%Creset' ..@{u})
  outgoing = !(git fetch --quiet && git log --pretty=format:'%C(yellow)%h %C(white)- %C(red)%an %C(white)- %C(cyan)%d%Creset %s %C(white)- %ar%Creset' @{u}..)
  unstage = reset HEAD --
  undo = checkout --
  rollback = reset --soft HEAD~1
```
