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

# EXPLICAÇÕES

Exemplo de um confirmador:
  - a96c4c3
  - a96c4c3936dbaa78be7254eb7b6b9b86fc46adc0

O que é uma ramificação?

> As ramificações do Git são um indicador efetivo de um instantâneo de suas mudanças. Quando você quiser adicionar um novo recurso ou corrigir um bug—não importa o tamanho, grande ou pequeno—basta criar uma nova ramificação para encapsular as mudanças. Isso faz com que seja mais difícil um código instável ser mesclado com a base de código principal e dá a chance de você limpar seu histórico futuro antes de fazer a mesclagem na ramificação principal.  

# COMANDOS

`git init` - Cria um repositório Git vazio ou reinicialize um existente.

`git status` - Informa o estado das alterações do nosso projeto.

`git add [file]` - Adiciona ou atualiza mudanças para irem para o repositório.
`git add .` - Se quiser referenciar todos os arquivos use o " . ".

`git commit -m "message"` - Registra alterações no repositório.
`git commit -am "message"` - Atualiza o repositório e registra alterações no repositório ao mesmo tempo.

`git log` - Mostra os pontos na "linha do tempo" do repositório ( commit ).
`git log --oneline` - Mostra os pontos na "linha do tempo" de forma mais resumida.
`git log --abbrev-commit` - Ao vez de mostrar o confirmador com 40 caracteres, mostra apenas com 7 caracteres.
`git log --pretty=oneline` - Faz com que caiba tudo em uma linha.
`git log --graph` - Desenha uma representação gráfica dos commits no lado esquerdo da saída.

`git diff` - Mostra o que foi alterado em um arquivo, de vermelho o que foi excluído de verde o que foi adicionando.
Use o "git diff" antes de dar o "git add".

`git show` - Apresenta determinado ponto na "história" do nosso projeto.

`git branch` - Lista, cria ou exclui ramificações.

`git checkout [confirmador]` - Alterna ramificações ou restaura arquivos da árvore de trabalho.
`git checkout [arquivo_modificado]` - Descarta as mudanças feitas no arquivo. Use antes de dar o "git add".
`git checkout -b [minha-feature]` - Cria uma nova ramificação no nosso projeto.
`git checkout master` - Vai para a ramificação master.
`git checkout [minha_ramificação]` - Vai para a ramificação criada pelo desenvolvedor.

`git reset HEAD` - Remove um arquivo adicionado pelo "git add". Usar depois do "git add" e antes do "git commit"
  `git reset --hard [confirmador]` - Remove um commit.

`git merge [minha_ramificação]` - Faz a fusão de uma ramificação x com a ramificação master. Para fazer a fusão você tem que estar na ramificação master.

`git remote` - Verifica se existe um repositório remoto.

`git push` - Envia alterações locais para o repositório remoto.

`git clone` - clonar um projeto / repositório.

`git pull` - Puxa do repositório remoto.

# ALIAS
Você pode criar alias para os comandos do git, basta ir no arquivo ".gitconfig" e definir seus alias.

Alias que eu gosto de usar:

[alias] <br>
  i = init <br>
  a = add <br>
  ci = commit <br>
  co = checkout <br>
  cm = checkout master <br>
  cb = checkout -b <br>
  st = status -sb <br>
  sf = show --name-only <br>
  pom = push origin master -u <br>
  ps = push <br>
  lg = log --pretty=format:'%Cred%h%Creset %C(bold)%cr%Creset %Cgreen<%an>%Creset %s' --max-count=30 <br>
  incoming = !(git fetch --quiet && git log --pretty=format:'%C(yellow)%h %C(white)- %C(red)%an %C(white)- %C(cyan)%d%Creset %s %C(white)- %ar%Creset' ..@{u}) <br>
  outgoing = !(git fetch --quiet && git log --pretty=format:'%C(yellow)%h %C(white)- %C(red)%an %C(white)- %C(cyan)%d%Creset %s %C(white)- %ar%Creset' @{u}..) <br>
  unstage = reset HEAD -- <br>
  undo = checkout -- <br>
  rollback = reset --soft HEAD~1 <br>
