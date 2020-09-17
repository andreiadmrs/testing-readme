## Cmandos

- **`git init`** - Cria um repositório Git vazio ou reinicialize um existente. <br>

- **`git status`** - Informa o estado das alterações do nosso projeto. <br>

- **`git add [file]`** - Adiciona ou atualiza mudanças para irem para o repositório.
- **`git add .`** - Você pode adicionar todos os arquivo usando o " . ". <br>

- **`git commit -m "message"`** - Registra alterações no repositório.
- **`git commit -am "message"`** - Atualiza o repositório e registra alterações no repositório ao mesmo tempo. <br>

- **`git log`** - Mostra os pontos na "linha do tempo" do repositório ( commit ).
- **`git log --oneline`** - Mostra os pontos na "linha do tempo" de forma mais resumida.
- **`git log --abbrev-commit`** - Ao vez de mostrar o hash com 40 caracteres, mostra apenas com 7 caracteres.
- **`git log --pretty=oneline`** - Faz com que caiba tudo em uma linha.
- **`git log --graph`** - Desenha uma representação gráfica dos commits no lado esquerdo da saída. <br>

- **`git diff`** - Mostra o que foi alterado em um arquivo, de vermelho o que foi excluído de verde o que foi adicionando.
Use o "git diff" antes de dar o "git add". <br>

- **`git show`** - Apresenta o último ponto na "história" do nosso projeto.
- **`git show [hash]`** - Apresenta determinado ponto na "história" do nosso projeto. <br>

- **`git branch`** - Lista, cria ou exclui ramificações. <br>

- **`git checkout [hash]`** - Alterna ramificações ou restaura arquivos da árvore de trabalho.
- **`git checkout [arquivo_modificado]`** - Descarta as mudanças feitas no arquivo. Use antes de dar o "git add".
- **`git checkout -b [minha-feature]`** - Cria uma nova ramificação no nosso projeto.
- **`git checkout master`** - Vai para a ramificação master.
- **`git checkout [minha_ramificação]`** - Vai para a ramificação criada pelo desenvolvedor. <br>

- **`git reset HEAD`** - Remove um arquivo adicionado pelo "git add". Usar depois do "git add" e antes do "git commit".
- **`git reset --hard [hash]`** - Remove um commit. <br>

- **`git merge [minha_ramificação]`** - Faz a fusão de uma ramificação x com a ramificação master. Para fazer a fusão você tem que estar na ramificação master. <br>

- **`git remote`** - Verifica se existe um repositório remoto. <br>

- **`git push`** - Envia alterações locais para o repositório remoto. <br>

- **`git clone [link_repositório]`** - Clonar um projeto / repositório.  <br>

- **`git pull`** - Puxa do repositório remoto.
