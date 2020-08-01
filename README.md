# GIT E GITHUB

Guia prático para iniciantes.

### Instalação

https://git-scm.com/download

### Documentação

https://git-scm.com/doc

# CENAS

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

# COMANDOS

`git init` - Cria um repositório Git vazio ou reinicialize um existente.<br>

`git status` - Informa o estado das alterações do nosso projeto.<br>

`git add [file]` - Adiciona ou atualiza mudanças para irem para o repositório.<br>
`git add .` - Se quiser referenciar todos os arquivos use o " . ".<br>

`git commit -m "message"` - Registra alterações no repositório.<br>
`git commit -am "message"` - Atualiza o repositório e registra alterações no repositório ao mesmo tempo.<br>

`git log` - Mostra os pontos na "linha do tempo" do repositório ( commit ).<br>
`git log --oneline` - Mostra os pontos na "linha do tempo" de forma mais resumida.<br>
`git log --abbrev-commit` - Ao vez de mostrar o hash com 40 caracteres, mostra apenas com 7 caracteres.<br>
`git log --pretty=oneline` - Faz com que caiba tudo em uma linha.<br>
`git log --graph` - Desenha uma representação gráfica dos commits no lado esquerdo da saída.<br>

`git diff` - Mostra o que foi alterado em um arquivo, de vermelho o que foi excluído de verde o que foi adicionando.
Use o "git diff" antes de dar o "git add".<br>

`git show` - Apresenta o último ponto na "história" do nosso projeto.<br>
`git show [hash]` - Apresenta determinado ponto na "história" do nosso projeto.<br>

`git branch` - Lista, cria ou exclui ramificações.<br>

`git checkout [hash]` - Alterna ramificações ou restaura arquivos da árvore de trabalho.<br>
`git checkout [arquivo_modificado]` - Descarta as mudanças feitas no arquivo. Use antes de dar o "git add".<br>
`git checkout -b [minha-feature]` - Cria uma nova ramificação no nosso projeto.<br>
`git checkout master` - Vai para a ramificação master.<br>
`git checkout [minha_ramificação]` - Vai para a ramificação criada pelo desenvolvedor.<br>

`git reset HEAD` - Remove um arquivo adicionado pelo "git add". Usar depois do "git add" e antes do "git commit".<br>
`git reset --hard [hash]` - Remove um commit.<br>

`git merge [minha_ramificação]` - Faz a fusão de uma ramificação x com a ramificação master. Para fazer a fusão você tem que estar na ramificação master.<br>

`git remote` - Verifica se existe um repositório remoto.<br>

`git push` - Envia alterações locais para o repositório remoto.<br>

`git clone` - clonar um projeto / repositório.<br>

`git pull` - Puxa do repositório remoto.<br>

Exemplo de um hash:
  - a96c4c3
  - a96c4c3936dbaa78be7254eb7b6b9b86fc46adc0

O que é uma ramificação?

> As ramificações do Git são um indicador efetivo de um instantâneo de suas mudanças. Quando você quiser adicionar um novo recurso ou corrigir um bug—não importa o tamanho, grande ou pequeno—basta criar uma nova ramificação para encapsular as mudanças. Isso faz com que seja mais difícil um código instável ser mesclado com a base de código principal e dá a chance de você limpar seu histórico futuro antes de fazer a mesclagem na ramificação principal.  

# ALIAS
Você pode criar alias para os comandos do git, basta ir no arquivo ".gitconfig" e definir seus alias.

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
